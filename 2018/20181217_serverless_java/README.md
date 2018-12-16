# 主題：Serverless Java: Challenges and Triumphs

* 活動資訊
  * KKTIX: https://twjug.kktix.cc/events/twjug201812-02
  * Meetup: https://www.meetup.com/taiwanjug/events/256740237/

* fn project 相關資訊
  * github: https://github.com/fnproject

# 主題搶先看

搶先看內容取自 

> DAVID DELABASSEE - Serverless Java in Action with Fn!

https://www.youtube.com/watch?v=_6b8f29UJWM


## Serverless

* [3:32](https://youtu.be/_6b8f29UJWM?t=212)開始聊 serverless 
  * Function As a Service
    * Function：專注於一個功能，給他 input 就會有 output (或相對應的 side effect)
    * As a Service：受服務商管理的。讓開發者只要專心在開發 function，不用分心管理底層的事物。
* [5:35](https://youtu.be/_6b8f29UJWM?t=336) 什麼原因讓你會想用 Serverless 呢？
  * Management：我才不想花時間管理基礎建設跟 deploy 呢！
  * Scaling：(跟上面差不多的理由)
  * Billing：有用在會計費，沒人用就沒計費，很方便。
  * Development
* [7:11](https://youtu.be/_6b8f29UJWM?t=431) Serverless Today 來聊聊 Serverless 的現況唄！
  * Serverless is killing containers (真的假的!?)
* [7:50](https://youtu.be/_6b8f29UJWM?t=470) 對比 Java 採用率與 Serverless 市佔來分析目前 Java 在 Serverless 環境下的現況。
  * [Serverless by the numbers: 2018 report](https://serverless.com/blog/serverless-by-the-numbers-2018-data-report)
  * [10:40](https://youtu.be/_6b8f29UJWM?t=640) 3 大雲端平台 Serverless 對 Java 支援的情況
  * [When Web Companies Grow Up They Turn into Java shops](https://redmonk.com/jgovernor/2016/10/12/when-web-companies-grow-up-they-turn-into-java-shops/)
* [11:37](https://youtu.be/_6b8f29UJWM?t=697) Serverless Java
* [13:40](https://youtu.be/_6b8f29UJWM?t=820) Fn Open Source Project
  * 跑在 container 內 (docker)
  * apache v2 license
  * 只要有 docker 地方就能跑 (雲端、機房或你的筆電)
  * 對 java 支援相當好 (也支援多種熱門的語言)
  * functions 就是 docker containers
* [16:18](https://youtu.be/_6b8f29UJWM?t=978) Fn Java Function Development Kit
  * build time 與 runtime 的 docker image
  * junit 支援
  * maven 支援
  * flow (組裝多個 function)
* [17:25](https://youtu.be/_6b8f29UJWM?t=1045) Demo 時間
  * [18:14](https://youtu.be/_6b8f29UJWM?t=1094) `fn init --runtime java duke`
    * 建立出了 maven project
    * configuration 是 yaml 
    * [19:43](https://youtu.be/_6b8f29UJWM?t=1183) HelloFunction
    * [21:45](https://youtu.be/_6b8f29UJWM?t=1305) `fn deploy --verbose --app cluj`
    * [24:09](https://youtu.be/_6b8f29UJWM?t=1449)
        * `fn ls fn clju`
        * `cat in.json | fn invoke cluj duke`
    * [27:13](https://youtu.be/_6b8f29UJWM?t=1633) fn function 在雲端跑也是沒問題的
      * `fn use context oci` 切換 provider 至 oci，oci 是 context 名稱，是 oracle 的 cloud platform
* [29:37](https://youtu.be/_6b8f29UJWM?t=1777) Fn Flow 用來建立複雜的應用
  * Java 8 CompletableFuture API
  * [31:30](https://youtu.be/_6b8f29UJWM?t=1890) Fn Flow Demo
  * [33:47](https://youtu.be/_6b8f29UJWM?t=2027) Fn Flow Graph
* [36:38](https://youtu.be/_6b8f29UJWM?t=2198) Low Latency
  * [37:07](https://youtu.be/_6b8f29UJWM?t=2227) Respecting Resource Constraints (JVM 要相對應的修改)
    * JDK-8179498
    * JDK-8193710
    * JDK-8203357
    * JDK 11 - JEP 318: Epsilon (No-Op GC)
* [38:39](https://youtu.be/_6b8f29UJWM?t=2319) Start Fast
  * Class Data Sharing
  * AOT compilation
* [40:07](https://youtu.be/_6b8f29UJWM?t=2407) Run Small Images
  * jlink
  * Project Portola
  * [43:24](https://youtu.be/_6b8f29UJWM?t=2606) GrallVM




