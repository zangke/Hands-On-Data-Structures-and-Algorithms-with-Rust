# Chapter 02
## Setup
```sh
rustup install nightly
rustup toolchain list
rustup override set nightly
# rustup override set stable
cargo test
cargo bench
```

## criterion.rs
https://course.rs/test/benchmark.html
官方 benchmark 有两个问题，首先就是不支持 stable 版本的 Rust，其次是结果有些简单，缺少更详细的统计分布。
因此社区 benchmark 就应运而生，其中最有名的就是 criterion.rs，它有几个重要特性:
统计分析，例如可以跟上一次运行的结果进行差异比对
图表，使用 gnuplots 展示详细的结果图表
