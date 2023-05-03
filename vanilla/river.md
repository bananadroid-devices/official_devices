# Notes

- Vanilla only   
- CTS pass   
- user builds   

# Changelog

================================    
======== 2023 -05 - 03 =========    
================================    

 - sync to last source    
 - added serval optimizations and tweaks    

================================   
======== 2023 - 04 - 22 ========   
================================   

device/motorola/sdm632-common   

 - sdm632-common: setup 4GB zram   
 - sdm632-common: Use 2GB dalvik-heap config   
 - sdm632-common: props: Better RAM Management   
 - sdm632-common: Add smooth motion flag & prop   
 - sdm632-common: dsds: restart qcrild on data switch    
 - sdm632-common: init: restart qcrild on decryption   
 - sdm632-common: init: Apply aggressive write caching.    
 - sdm632-common: Disable sdm rotator downscaler   
 - sdm632-common: Disable blur on app launch   
 - sdm632-common: prop: Force disable iorapd    
 - sdm632-common: add more iorapd props   
 - sdm632-common: props: enable gfx accel   
 - sdm632-common: rootdir: Add offline charging LED indicator    
 - sdm632-common: props: Disable Skia tracing by default    
 - sdm632-common: props: enable vsync and disable backpressure    
 - sdm632-common: wlan: Relax WiFi   
 - sdm632-common: Speed profile services    
 - sdm632-common: Add some Android GO configuration   
 - sdm632-common: Use speed tuning for performance critical applications    
 - sdm632-common: props: Adapt unsignaled buffer latch property    
 - sdm632-common: set dex2oat filter = quicken    
 - sdm632-common: Optimize package manager dexopt properties    
 - sdm632-common: Use dex2oat64    
 - sdm632-common: shorten wait time to optimize shutdown time     
 - sdm632-common: power: Set all 8 cores online    
 - sdm632-common: Disable HWC composition strategy prediction    
 - sdm632-common: Disable continuous transaction tracing on all build types    
 - sdm632-common: Disable HWC overlay    
 - sdm632-common: Disable Async MTE on System Server    
 - sdm632-common: Enable LTE_CA workaround    
 - sdm632-common: Enable use of PerformanceHintManager for HWUI     
 - sdm632-common: Disable SysUI blur    
 - sdm632-common: init: Enable Suspend-To-RAM system suspend mode     
 - sdm632-common: overlay: Improve pinner configuration    
 - sdm632-common: Remove duplicate camera property     

kernel/motorola/sdm632

 - mm: swap: swap pages one at a time     
 - tcp: Increase max connections to accept     
 - msm: kgsl: Report correct GPU frequency in sysfs     
 - sched: Do not give sleepers 50% more runtime     
 - cfq-iosched: Apply tunes from Pixel 4     
 - blk-cgroup: filter background cgroup out     
 - fs: f2fs: enlarge min_fsync_blocks to 20     
 - msm: kgsl: Report correct GPU frequency for clock_mhz     
 - ICE, pfk: fix to set dio_inode precisely     
 - FROMGIT: dm: do not allow readahead to limit IO size    
 - f2fs, dm-default-key: should skip dm-default-key only for FBE blocks     
 - f2fs: don't allow any writes on readonly mount     
 - dm verity fec: remove redundant unlikely annotation     
 - dm verity fec: fix GFP flags used with mempool_alloc()     
 - sdcardfs: fix wrong ENOENT when creating a file     
 - kernel: time: reduce ntp wakeups     
 - f2fs: set ioprio of GC kthread to idle    
 - techpack: display: Disable debug logging macros     
 - f2fs: Remove additional tracings added by CAF    
 - f2fs: Fix deadlock between f2fs_quota_sync and block_operation    
 - drivers: gpu: msm: Remove tracing    
 - arm64: crypto: add NEON accelerated XOR implementation     
 - Kernel/sched: Reduce latency for better responsiveness     
 - msm: kgsl: Dispatch commands using a master kthread     
 - [BACKPORT] msm: kgsl: Do GPU bus governor management     
 - [BACKPORT] PM / devfreq: Make update_devfreq() public    
 - [BACKPORT] adreno_tz: Remove partner devfreq management    
 - msm: kgsl: Don't busy wait for fenced GMU writes when possible    
 - sched/fair: Move the PELT constants into a generated header    
 - sched/Documentation: Add 'sched-pelt' tool     
 - FROMLIST: sched/fair: add support to tune PELT ramp/decay timings     
 - sched/fair: Increase PELT accuracy for small tasks    
 - arm64/configs: Switch to 16ms half-life PELT     
 - arm64/configs: Enable FAT UTF-8 option by default    
 - f2fs/gc: Reduce GC thread urgent sleep time to 50ms     
 - ashmem: Align slab caches to L1 cache line     
 - msm: Fix high load average from uninterruptible waits    
 - sched/fair: Avoid force newly idle load balance if have iowait task     
 - lib: zstd: Add kernel-specific API     
 - lib: zstd: Upgrade to latest upstream zstd version 1.4.10    
 - lib: zstd: Add cast to silence clang's -Wbitwise-instead-of-logical     
 - lib: zstd: Fix unused variable warning    
 - lib: zstd: Don't inline functions in zstd_opt.c     
 - lib: zstd: Don't add -O3 to cflags     
 - lib: zstd: Fix attribute declaration     
 - lib: zstd: Upgrade to latest upstream zstd version pre-1.5.2    
 - lib: zstd: Fix unknown type name size_t    
 - lib: zstd: Workaround duplicate symbols     
 - crypto/zstd.c: ZSTD_DEF_LEVEL switch to 1     
 - lib: zstd: Upstream codebase to v1.5.3 (dev branch)     
 - arm64/configs: Enable zstd compression algo config option    
 - zram: fix race between zram_reset_device() and disksize_store()     
 - zram: replace fsync_bdev with sync_blockdev     
 - zram_drv: allow reclaim on bio_alloc     
 - zram: do not waste zram_table_entry flags bits     
 - f2fs: add trim stop mechanism     
 - f2fs: enable fstrim to issue discard while using discard option    
 - arm64/configs: Disable CONFIG_DEBUG_ALIGN_RODATA    
 - cpufreq: Ensure the minimal frequency is lower than the maximal freq    

