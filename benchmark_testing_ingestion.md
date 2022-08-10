## Context
Benchmark the performance of the ingestion pipeline


| Operation | Number of nodes | Concurrency | Is Large | Time of execution with new code | Number of erred out |
| --- | --- | --- | --- | --- | --- |
| Insert | 100 | 10	| No | real0m10.579s user0m13.931s sys0m0.437s | 0 |
| Update | 100 | 10	| No | real0m1.740s user0m16.530s sys0m0.136s | 0 |
| Insert | 500 | 10	| No | real1m2.392s user1m11.486s sys0m1.532s | 0 |
| Update | 500 | 10	| No | real1m11.343s user1m11.984s sys0m1.730s | 0 |
| Insert | 1000 | 10 | No | real2m7.966s user2m23.792s sys0m2.753s | 0 |
| Update | 1000	| 10 | No | real2m18.504s user2m24.229s sys0m3.768s | 0 |
| Insert | 5000	| 50 | No | real3m28.962s user3m1.810s sys0m1.420s | 3605 |
| Update | 5000	| 50 | No | real5m17.567s user12m28.765s sys0m9.042s | 3803 |
| Insert | 10000 | 100 | yes | real20m56.567s user19m34.237s sys0m9.142s | 1436 |
| Update | 10000 | 100 | yes | real25m56.567s user19m34.237s sys0m24.142s | 1856 |
| Insert | 20000 | 200 | yes | real9m10.474s user66m4.175s sys0m28.368s | 19865 |
| Update | 20000 | 200 | yes | real8m4.448s user4m45.706s sys0m8.862s | 19883 |