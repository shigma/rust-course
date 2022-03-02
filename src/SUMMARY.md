# Rust语言圣经

[进入Rust编程世界](into-rust.md)
[AWS为何这么喜欢Rust?](usecases/aws-rust.md)
[避免从入门到放弃](sth-you-should-not-do.md)
[关于本书](about-book.md)

[快速查询入口](index-list.md)

## Getting started
- [寻找牛刀，以便小试](first-try/intro.md)
    - [安装Rust环境](first-try/installation.md)
    - [墙推VSCode!](first-try/editor.md)
    - [认识Cargo](first-try/cargo.md)
    - [不仅仅是Hello world](first-try/hello-world.md)

## Rust学习三部曲

- [Rust基础入门](basic/intro.md)
    - [变量绑定与解构](basic/variable.md)
    - [基本类型](basic/base-type/index.md)
        - [数值类型](basic/base-type/numbers.md)
        - [字符、布尔、单元类型](basic/base-type/char-bool.md)
        - [语句与表达式](basic/base-type/statement-expression.md)
        - [函数](basic/base-type/function.md)
    - [所有权和借用](basic/ownership/index.md)
        - [所有权](basic/ownership/ownership.md)
        - [引用与借用](basic/ownership/borrowing.md)
    - [复合类型](basic/compound-type/intro.md)
        - [字符串与切片](basic/compound-type/string-slice.md)
        - [元组](basic/compound-type/tuple.md)
        - [结构体](basic/compound-type/struct.md)
        - [枚举](basic/compound-type/enum.md)
        - [数组](basic/compound-type/array.md)
    - [流程控制](basic/flow-control.md)
    - [模式匹配](basic/match-pattern/intro.md)
        - [match和if let](basic/match-pattern/match-if-let.md)
        - [解构Option](basic/match-pattern/option.md)
        - [模式适用场景](basic/match-pattern/pattern-match.md)
        - [全模式列表](basic/match-pattern/all-patterns.md)
    - [方法Method](basic/method.md)
    - [泛型和特征](basic/trait/intro.md)
        - [泛型Generics](basic/trait/generic.md)
        - [特征Trait](basic/trait/trait.md)
        - [特征对象](basic/trait/trait-object.md)
        - [进一步深入特征](basic/trait/advance-trait.md)
    - [集合类型](basic/collections/intro.md)
        - [动态数组Vector](basic/collections/vector.md)
        - [KV存储HashMap](basic/collections/hashmap.md)
    - [类型转换](basic/converse.md)
    - [返回值和错误处理](basic/result-error/intro.md)
        - [panic深入剖析!](basic/result-error/panic.md)
        - [返回值Result和?](basic/result-error/result.md)
    - [包和模块](basic/crate-module/intro.md)
        - [包Crate](basic/crate-module/crate.md)
        - [模块Module](basic/crate-module/module.md)
        - [使用use引入模块及受限可见性](basic/crate-module/use.md)
    - [注释和文档](basic/comment.md)
    - [格式化输出](basic/formatted-output.md)
- [Rust高级进阶](advance/intro.md)
    - [生命周期](advance/lifetime/intro.md)
        - [认识生命周期](advance/lifetime/basic.md)
        - [深入生命周期](advance/lifetime/advance.md)
        - [&'static 和 T: 'static](advance/lifetime/static.md)
        <!-- - [一些关于生命周期的误解 todo](advance/lifetime/misconceptions.md) -->
    - [函数式编程: 闭包、迭代器](advance/functional-programing/intro.md)
        - [闭包Closure](advance/functional-programing/closure.md)
        - [迭代器Iterator](advance/functional-programing/iterator.md)
    - [深入类型](advance/into-types/intro.md)
      - [newtype 和 类型别名](advance/into-types/custom-type.md)
      - [Sized 和不定长类型 DST](advance/into-types/sized.md)
      - [枚举和整数](advance/into-types/enum-int.md)
    - [智能指针](advance/smart-pointer/intro.md)
        - [Box<T>堆对象分配](advance/smart-pointer/box.md)
        - [Deref解引用](advance/smart-pointer/deref.md)
        - [Drop释放资源](advance/smart-pointer/drop.md)
        - [Rc与Arc实现1vN所有权机制](advance/smart-pointer/rc-arc.md)
        - [Cell与RefCell内部可变性](advance/smart-pointer/cell-refcell.md)
    - [循环引用与自引用](advance/circle-self-ref/intro.md)
        - [Weak与循环引用](advance/circle-self-ref/circle-reference.md)
        - [结构体中的自引用](advance/circle-self-ref/self-referential.md))
    - [多线程并发编程](advance/concurrency-with-threads/intro.md)
        - [并发和并行](advance/concurrency-with-threads/concurrency-parallelism.md)
        - [使用多线程](advance/concurrency-with-threads/thread.md)
        - [线程同步：消息传递](advance/concurrency-with-threads/message-passing.md)
        - [线程同步：锁、Condvar和信号量](advance/concurrency-with-threads/sync1.md)
        - [线程同步：Atomic原子操作与内存顺序](advance/concurrency-with-threads/sync2.md)
        - [基于Send和Sync的线程安全](advance/concurrency-with-threads/send-sync.md)
        - [实践应用：多线程Web服务器 todo](advance/concurrency-with-threads/web-server.md)
    - [全局变量](advance/global-variable.md)
    - [错误处理](advance/errors.md)
    
    - [Unsafe Rust](advance/unsafe/intro.md)
      - [五种兵器](advance/unsafe/superpowers.md)
      - [内联汇编 todo](advance/unsafe/inline-asm.md)
    - [Macro宏编程](advance/macro.md)
    <!-- - [SIMD todo](advance/simd.md) -->
    <!-- - [高阶特征约束(HRTB) todo](advance/hrtb.md) -->

## 专题内容,每个专题都配套一个小型项目进行实践  
- [自动化测试](test/intro.md)
    - [编写测试及控制执行](test/write-tests.md)
    - [单元测试和集成测试](test/unit-integration-test.md)
    - [断言assertion](test/assertion.md)
    - [用Github Actions进行持续集成](test/ci.md)
    - [基准测试benchmark](test/benchmark.md)

- [async/await异步编程](async/intro.md)
  - [async编程入门](async/getting-started.md)
  - [底层探秘: Future执行与任务调度](async/future-excuting.md)
  - [定海神针Pin和Unpin](async/pin-unpin.md)
  - [async/await和Stream流处理](async/async-await.md)
  - [同时运行多个Future](async/multi-futures-simultaneous.md)
  - [一些疑难问题的解决办法](async/pain-points-and-workarounds.md)
  - [实践应用：Async Web服务器](async/web-server.md)
  
- [Tokio使用指南](tokio/intro.md)
    - [tokio概览](tokio/overview.md)
    - [使用初印象](tokio/getting-startted.md)
    - [创建异步任务](tokio/spawning.md)
    - [共享状态](tokio/shared-state.md)
    - [消息传递](tokio/channels.md)
    - [I/O](tokio/io.md)
    - [解析数据帧](tokio/frame.md)
    - [深入async](tokio/async.md)
    - [select](tokio/select.md)
    - [类似迭代器的Stream](tokio/stream.md))   
    - [优雅的关闭](tokio/graceful-shutdown.md)
    - [异步跟同步共存](tokio/bridging-with-sync.md)
 
- [Cargo使用指南](cargo/intro.md)
    - [上手使用](cargo/getting-started.md)
    - [基础指南](cargo/guide/intro.md)
      - [为何会有Cargo](cargo/guide/why-exist.md)
      - [下载并构建Package](cargo/guide/download-package.md)
      - [添加依赖](cargo/guide/dependencies.md)
      - [Package目录结构](cargo/guide/package-layout.md)
      - [Cargo.toml vs Cargo.lock](cargo/guide/cargo-toml-lock.md)
      - [测试和CI](cargo/guide/tests-ci.md)
      - [Cargo缓存](cargo/guide/cargo-cache.md)
      - [Build缓存](cargo/guide/build-cache.md)
    - [进阶指南 doing](cargo/reference/intro.md)
        - [指定依赖项](cargo/reference/specify-deps.md)
        - [依赖覆盖](cargo/reference/deps-overriding.md)
        - [Cargo.toml清单详解](cargo/reference/manifest.md)
        - [Cargo Target](cargo/reference/cargo-target.md)
        - [工作空间Workspace](cargo/reference/workspaces.md)
        - [条件编译Features](cargo/reference/features/intro.md)
          - [Features示例](cargo/reference/features/examples.md)
        - [发布配置Profile](cargo/reference/profiles.md)
        - [通过config.toml对Cargo进行配置](cargo/reference/configuration.md)
        - [发布到crates.io](cargo/reference/publishing-on-crates.io.md)
        - [构建脚本 todo](cargo/reference/build-script/intro.md)
          - [构建脚本示例 todo](cargo/reference/build-script/examples.md)

- [易混淆概念解析](confonding/intro.md)
    - [切片和切片引用](confonding/slice.md)
    - [String、&str 和 str](confonding/string.md)
    - [原生指针、引用和智能指针 todo](confonding/pointer.md)
    - [作用域、生命周期和 NLL todo](confonding/lifetime.md)
    - [move、Copy和Clone todo](confonding/move-copy.md)

- [对抗编译检查 doing](fight-with-compiler/intro.md)
    - [幽灵数据(todo)](fight-with-compiler/phantom-data.md)
    - [生命周期](fight-with-compiler/lifetime/intro.md)
        - [生命周期过大-01](fight-with-compiler/lifetime/too-long1.md)
        - [生命周期过大-02](fight-with-compiler/lifetime/too-long2.md)
        - [循环中的生命周期](fight-with-compiler/lifetime/loop.md)
        - [闭包碰到特征对象-01](fight-with-compiler/lifetime/closure-with-static.md)
    - [重复借用](fight-with-compiler/borrowing/intro.md)
        - [同时在函数内外使用引用](fight-with-compiler/borrowing/ref-exist-in-out-fn.md)
        - [智能指针引起的重复借用错误](fight-with-compiler/borrowing/borrow-distinct-fields-of-struct.md)
    - [类型未限制(todo)](fight-with-compiler/unconstrained.md)


- [Rust常见陷阱](pitfalls/index.md)
    - [for循环中使用外部数组](pitfalls/use-vec-in-for.md)
    - [线程类型导致的栈溢出](pitfalls/stack-overflow.md)
    - [算术溢出导致的panic](pitfalls/arithmetic-overflow.md)
    - [闭包中奇怪的生命周期](pitfalls/closure-with-lifetime.md)
    - [可变变量不可变？](pitfalls/the-disabled-mutability.md)
    - [可变借用失败引发的深入思考](pitfalls/multiple-mutable-references.md)
    - [不太勤快的迭代器](pitfalls/lazy-iterators.md)
    - [奇怪的序列x..y](pitfalls/weird-ranges.md)
    - [无处不在的迭代器](pitfalls/iterator-everywhere.md)
    - [线程间传递消息导致主线程无法结束](pitfalls/main-with-channel-blocked.md)

- [Rust最佳实践 doing](practice/intro.md)
    - [日常开发三方库精选](practice/third-party-libs.md)
    - [命名规范](practice/naming.md)
    - [代码开发实践 todo](practice/best-pratice.md)
    - [日志记录 todo](practice/logs.md)
    - [可观测性监控 todo](practice/observability.md)
  
<!-- - [如何实现一个链表 todo]() -->
  
- [Rust性能剖析 todo](profiling/intro.md)  
  - [深入内存 todo](profiling/memory/intro.md)
      - [指针和引用 todo](profiling/memory/pointer-ref.md)
      - [未初始化内存 todo](profiling/memory/uninit.md)
      - [内存分配 todo](profiling/memory/allocation.md)
      - [内存布局 todo](profiling/memory/layout.md)
      - [虚拟内存 todo](profiling/memory/virtual.md)   
  - [性能调优 doing](profiling/performance/intro.md)
      - [字符串操作性能](profiling/performance/string.md)
      - [深入理解move](profiling/performance/deep-into-move.md)
      - [糟糕的提前优化 todo](profiling/performance/early-optimise.md)
      - [Clone和Copy todo](profiling/performance/clone-copy.md)
      - [减少Runtime check(todo)](profiling/performance/runtime-check.md)
      - [CPU缓存性能优化 todo](profiling/performance/cpu-cache.md)
      - [计算性能优化 todo](profiling/performance/calculate.md)
      - [堆和栈 todo](profiling/performance/heap-stack.md)
      - [内存allocator todo](profiling/performance/allocator.md)
      - [常用性能测试工具 todo](profiling/performance/tools.md)
      - [Enum内存优化 todo](profiling/performance/enum.md)
  - [编译优化 todo](profiling/compiler/intro.md)
      - [LLVM todo](profiling/compiler/llvm.md)
      - [常见属性标记 todo](profiling/compiler/attributes.md)
      - [提升编译速度 todo](profiling/compiler/speed-up.md)
      - [编译器优化 todo](profiling/compiler/optimization/intro.md)
        - [Option枚举 todo](profiling/compiler/optimization/option.md)

- [标准库解析 todo](std/intro.md)
    - [标准库使用最佳时间 todo](std/search.md)
    - [Vector常用方法 todo](std/vector.md)
    - [HashMap todo](std/hashmap.md)
    - [Iterator常用方法 todo](std/iterator.md)

- [Ctrl-C/V: 编程常用代码片段 todo](cases/intro.md)
  - [命令行解析 todo](cases/cmd.md)
  - [配置文件解析 todo](cases/config.md)
  - [编解码 todo](cases/encoding/intro.md)
    - [JSON](cases/encoding/json.md)
    - [CSV](cases/encoding/csv.md)
    - [protobuf](cases/encoding/protobuf.md)
  - [文件系统 todo](cases/file/intro.md)
    - [文件读写](cases/file/file.md)
    - [目录操作](cases/file/dir.md)
  - [网络通信 todo](cases/protocol/intro.md)
    - [HTTP](cases/protocol/http.md)
    - [TCP](cases/protocol/tcp.md)
    - [UDP](cases/protocol/udp.md)
    - [gRPC](cases/protocol/grpc.md)
  - [数据库访问 todo](cases/database.md)
  - [正则表达式 todo](cases/regexp.md)
  - [加密解密 todo](cases/crypto.md)
  - [时间日期](cases/date.md)
  - [开发调试 todo](cases/dev/intro.md)
    - [日志](cases/dev/logs.md)
    - [性能分析](cases/dev/profile.md)
    
<!-- 
- [Rust区块链入门]()
- [Rust游戏开发入门]()
- [Rust前端开发入门]()
- [Rust和WASM]() -->

## 附录
- [附录](appendix/intro.md)
    - [A-关键字](appendix/keywords.md)
    - [B-运算符与符号](appendix/operators.md)
    - [C-表达式](appendix/expressions.md)
    - [D-派生特征 trait](appendix/derive.md)
    - [E-prelude 模块 todo](appendix/prelude.md)
    - [F-Rust 版本说明](appendix/rust-version.md)
    - [G-Rust 更新版本列表](appendix/rust-versions/intro.md)
      - [1.58](appendix/rust-versions/1.58.md)
      - [1.59](appendix/rust-versions/1.59.md)
