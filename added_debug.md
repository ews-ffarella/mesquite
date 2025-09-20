`ABL_MF_DEBUG` in src/MappingFunction/MappingFunction.cpp
`ABL_PRISM_QA_TRACE` in src/QualityAssessor/QualityAssessor.cpp
`ABL_MQ_DEBUG` in src/QualityMetric/TMP/TMPQualityMetric.cpp
`MQ_DEBUG` in src/QualityMetric/TMP/TQualityMetric.cpp
`ABL_JAC_TRACE` in src/TargetCalculator/TargetCalculator.cpp
`ABL_PGM_GRAD_DEBUG` in src/mesquite/PrismaticGaralloMetric.cpp

```bash
export ABL_MF_DEBUG=1
export ABL_PRISM_QA_TRACE=1
export ABL_MQ_DEBUG=1
export MQ_DEBUG=1
export ABL_JAC_TRACE=1
export ABL_PGM_GRAD_DEBUG=1
```

```bash
unset ABL_MF_DEBUG
unset ABL_PRISM_QA_TRACE
unset ABL_MQ_DEBUG
unset MQ_DEBUG
unset ABL_JAC_TRACE
unset ABL_PGM_GRAD_DEBUG
```
cd /home/ffarella/EWS/mes01 && ./build/bin/test_garallo_metric_test_single_prism --gtest_filter="*OptimizationWithScaleneBase*" 2<&1 | tee test.log