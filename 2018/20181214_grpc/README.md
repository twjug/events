# 主題：Fast and Efficient Microservices with gRPC

* 活動資訊：[Fast and Efficient Microservices with gRPC](https://twjug.kktix.cc/events/twjug201812-01)
* gRPC 官方資源
  * [Quick Start :: Java](https://grpc.io/docs/quickstart/java.html)
  * [github :: grpc-java](https://github.com/grpc/grpc-java)

## 前言

這份素材是活動 `Fast and Efficient Microservices with gRPC` 的初階材料，若聽眾已經能完成下列事項，那可以略過此份素材：

* 將撰寫好的 protobuf idl (.proto) 檔編譯為 java source code，並產生 grpc stubs
* 使用 maven 或 gradle 編譯 grpc 專案

## gRPC 簡易上手篇

在初開始學習用 gRPC 時，看了網官的 `Quick Start :: Java` 但還是不知道如何下手，特別是想要建立 gradle 專案時，看了一堆眼花撩亂的 DSL 想著該由哪開始好呢？這也是為什麼試著提供『又』一篇的簡易上手文件。