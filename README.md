# GPU_Hunter

In this repo, I recall all the memory types and its performance, so you can figure out how your type of ddr/gddr ram succeed others.

| 内存类名  | JEDEC规范 | 核心频率MHz | 边沿 | 预读取系数 | 等效频率MT/s     =核心频率*预读取系数 | 位宽bit/Transfer | 单通道接口速率GB/s     =等效频率*位宽 | 双通道接口速率GB/s |             |
| --------- | --------- | ----------- | ---- | ---------- | ------------------------------------- | ---------------- | ------------------------------------- | ------------------ | ----------- |
| SDRAM     | PC66      | 67          | 单边 | 1          | 67                                    | 64               | 0.5                                   | NaN                |             |
| SDRAM     | PC100     | 100         | 单边 | 1          | 100                                   | 64               | 0.8                                   | NaN                |             |
| SDRAM     | PC133     | 133         | 单边 | 1          | 133                                   | 64               | 1.0                                   | NaN                |             |
| Rambus    | PC800     | 400         | 双边 | 2          | 800                                   | 16               | 1.6                                   | 3.1                |             |
| Rambus    | PC1066    | 533         | 双边 | 2          | 1067                                  | 16               | 2.1                                   | 4.2                |             |
| DDR-200   | PC1600    | 100         | 双边 | 2          | 200                                   | 64               | 1.6                                   | 3.1                |             |
| DDR-266   | PC2100    | 133         | 双边 | 2          | 267                                   | 64               | 2.1                                   | 4.2                |             |
| DDR-333   | PC2700    | 167         | 双边 | 2          | 333                                   | 64               | 2.6                                   | 5.2                |             |
| DDR-400   | PC3200    | 200         | 双边 | 2          | 400                                   | 64               | 3.1                                   | 6.3                |             |
| DDR2-400  | PC2-3200  | 100         | 双边 | 4          | 400                                   | 64               | 3.1                                   | 6.3                |             |
| DDR2-533  | PC2-4200  | 133         | 双边 | 4          | 533                                   | 64               | 4.2                                   | 8.3                |             |
| DDR2-667  | PC2-5300  | 167         | 双边 | 4          | 667                                   | 64               | 5.2                                   | 10.4               |             |
| DDR2-800  | PC2-6400  | 200         | 双边 | 4          | 800                                   | 64               | 6.3                                   | 12.5               |             |
| DDR2-1066 | PC2-8500  | 267         | 双边 | 4          | 1067                                  | 64               | 8.3                                   | 16.7               | 三星规范    |
| DDR3-800  | PC3-6400  | 100         | 双边 | 8          | 800                                   | 64               | 6.3                                   | 12.5               |             |
| DDR3-1066 | PC3-8500  | 133         | 双边 | 8          | 1067                                  | 64               | 8.3                                   | 16.7               |             |
| DDR3-1333 | PC3-10600 | 167         | 双边 | 8          | 1333                                  | 64               | 10.4                                  | 20.8               |             |
| DDR3-1600 | PC3-12800 | 200         | 双边 | 8          | 1600                                  | 64               | 12.5                                  | 25.0               |             |
| DDR3-1866 | PC3-14900 | 233         | 双边 | 8          | 1867                                  | 64               | 14.6                                  | 29.2               |             |
| DDR3-2133 | PC3-17000 | 267         | 双边 | 8          | 2133                                  | 64               | 16.7                                  | 33.3               |             |
| DDR4-1600 | PC4-1600  | 100         | 双边 | 16         | 1600                                  | 64               | 12.5                                  | 25.0               |             |
| DDR4-1866 | PC4-1866  | 117         | 双边 | 16         | 1867                                  | 64               | 14.6                                  | 29.2               |             |
| DDR4-2133 | PC4-2133  | 133         | 双边 | 16         | 2133                                  | 64               | 16.7                                  | 33.3               |             |
| DDR4-2400 | PC4-2400  | 150         | 双边 | 16         | 2400                                  | 64               | 18.8                                  | 37.5               |             |
| DDR4-2666 | PC4-2666  | 167         | 双边 | 16         | 2667                                  | 64               | 20.8                                  | 41.7               |             |
| DDR4-3200 | PC4-3200  | 200         | 双边 | 16         | 3200                                  | 64               | 25.0                                  | 50.0               |             |
| DDR4-3600 | PC4-3600  | 225         | 双边 | 16         | 3600                                  | 64               | 28.1                                  | 56.3               | 非JEDEC规范 |
| DDR4-3733 | PC4-3733  | 233         | 双边 | 16         | 3733                                  | 64               | 29.2                                  | 58.3               | 非JEDEC规范 |
| DDR4-4266 | PC4-4266  | 267         | 双边 | 16         | 4267                                  | 64               | 33.3                                  | 66.7               | 非JEDEC规范 |
| DDR5-3200 | PC5-3200  | 100         | 双边 | 32         | 3200                                  | 64               | 25.0                                  | 50.0               | 尚未发布    |
| DDR5-4266 |           | 133         | 双边 | 32         | 4267                                  | 64               | 33.3                                  | 66.7               | 尚未发布    |
| DDR5-4800 | PC5-4800  | 150         | 双边 | 32         | 4800                                  | 64               | 37.5                                  | 75.0               | 尚未发布    |
| DDR5-5333 |           | 167         | 双边 | 32         | 5333                                  | 64               | 41.7                                  | 83.3               | 尚未发布    |
| DDR5-6400 | PC5-6400  | 200         | 双边 | 32         | 6400                                  | 64               | 50.0                                  | 100.0              | 尚未发布    |
| DDR5-7466 |           | 233         | 双边 | 32         | 7467                                  | 64               | 58.3                                  | 116.7              | 尚未发布    |
| DDR5-8533 |           | 267         | 双边 | 32         | 8533                                  | 64               | 66.7                                  | 133.3              | 尚未发布    |



Also, I read almost all NVIDIA white papers, and make a collection of its GPU architecture, and find a relationship among GPU/GPC/TPC/SM/CUDA, so you can figure out which GPU is the best deal.
![](media/image7.png){width="5.768055555555556in" height="4.345833333333333in"}
