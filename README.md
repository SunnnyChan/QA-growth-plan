# KS-QA
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)

![](_pic/QA.png)

QA
=================

   * [<a href="_pic/QA-capacity-model.png">QA 能力模型</a>](#qa-能力模型)
   * [<a href="SQA/SQ.md">软件质量</a>](#软件质量)
      * [软件质量模型](#软件质量模型)
   * [<a href="SQA/SQA.md">软件质量保证</a>](#软件质量保证)
   * [测试](#测试)
      * [<a href="Testing/Basic/README.md">测试基础</a>](#测试基础)
         * [<a href="Testing/Basic/README.md">测试原则</a>](#测试原则)
         * [<a href="Testing/Basic/README.md">测试策略</a>](#测试策略)
         * [<a href="Testing/Basic/README.md">测试用例</a>](#测试用例)
      * [<a href="Testing/UnitTest/README.md">单元测试(Unit Testing)</a>](#单元测试unit-testing)
         * [<a href="Testing/UnitTest/Java/Spock/README.md">Java - Spock</a>](#java---spock)
         * [Java - JUnit](#java---junit)
         * [Java - TestNG](#java---testng)
         * [Java - Mock - Mockito](#java---mock---mockito)
      * [<a href="Testing/APIsTest/README.md">接口测试(APIs Testing)</a>](#接口测试apis-testing)
      * [<a href="Testing/EndToEnd-Test/README.md">端到端测试(End-to-End Testing)</a>](#端到端测试end-to-end-testing)
      * [<a href="Testing/DataTest/README.md">数据测试</a>](#数据测试)
      * [配置测试](#配置测试)
      * [<a href="Testing/AutoTest/README.md">自动化测试</a>](#自动化测试)
      * [<a href="ET/README.md">探索式测试（Exploratory Test）</a>](#探索式测试exploratory-test)
      * [<a href="">基于交互的测试(Interaction-Based Testing)</a>](#基于交互的测试interaction-based-testing)
         * [<a href="Testing/InteractionBasedTest/Mock/README.md">Mock</a>](#mock)
      * [<a href="Testing/PropertyBasedTest/README.md">基于属性的测试(Property-Based Testing)</a>](#基于属性的测试property-based-testing)
      * [<a href="">模糊测试(Fuzzing Testing)</a>](#模糊测试fuzzing-testing)
      * [<a href="MutationTest/README.md">变异测试(Mutation Testing)</a>](#变异测试mutation-testing)
      * [<a href="Testing/AITest/README.md">智能测试(AI Testing)</a>](#智能测试ai-testing)
      * [精准测试](#精准测试)
   * [<a href="CodeReview/README.md">代码评审（Code Review)</a>](#代码评审code-review)
   * [<a href="CodeAnalysis/README.md">代码分析（Code Analysis）</a>](#代码分析code-analysis)
      * [<a href="CodeAnalysis/StaticAnalysis/README.md">静态代码检查(Code Static Inspect)</a>](#静态代码检查code-static-inspect)
      * [<a href="CodeAnalysis/CodeDiff/README.md">代码差异分析</a>](#代码差异分析)
      * [<a href="CodeAnalysis/Java/README.md">Java 代码分析</a>](#java-代码分析)
   * [<a href="QualityAnalysis/README.md">质量分析</a>](#质量分析)
      * [可测性分析](#可测性分析)
      * [<a href="QualityAnalysis/CodeCoverage/README.md">测试代码覆盖率分析（Code Coverage - 已有代码被测试了吗？</a>](#测试代码覆盖率分析code-coverage---已有代码被测试了吗)
         * [<a href="QualityAnalysis/CodeCoverage/Jacoco.md">Java - Jacoco</a>](#java---jacoco)
      * [测试有效性分析 - 已有代码测好了吗？](#测试有效性分析---已有代码测好了吗)
      * [业务覆盖率分析 - 还有哪些代码要写？](#业务覆盖率分析---还有哪些代码要写)
   * [<a href="Perf/README.md">性能</a>](#性能)
      * [<a href="Perf/PerfTest/README.md">性能测试</a>](#性能测试)
      * [<a href="Perf/PerfAnalysis/README.md">性能分析</a>](#性能分析)
      * [<a href="Perf/LinuxPerf/README.md">Linux 性能</a>](#linux-性能)
         * [<a href="https://github.com/SunnnyChan/sc.ebooks/tree/master/programme/profile/BPF-Perf">《BPF Performance Tools》</a>](#bpf-performance-tools)
      * [Systems Performance](#systems-performance)
         * [<a href="https://github.com/SunnnyChan/sc.ebooks/tree/master/programme/profile/sys-performance">《性能之巅：洞悉系统、企业和云计算》(Systems Performance: Enterprise and the Cloud)</a>](#性能之巅洞悉系统企业和云计算systems-performance-enterprise-and-the-cloud)
   * [稳定性](#稳定性)
      * [故障演练](#故障演练)
   * [<a href="QualityConsciousness/README.md">质量意识</a>](#质量意识)
      * [测试服务化 -  “把简单留给开发者，把复杂留给工具。”](#测试服务化----把简单留给开发者把复杂留给工具)
      * [测试认证](#测试认证)
   * [<a href="QualityPlatform/README.md">质量平台</a>](#质量平台)
   * [探索](#探索)
      * [<a href="https://en.wikipedia.org/wiki/Concolic_testing" rel="nofollow">Concolic Testing</a>](#concolic-testing)
   * [Reference](#reference)
      * [<a href="https://www.cnblogs.com/kenfang/articles/4307935.html" rel="nofollow">软件测试中英文词汇汇总表</a>](#软件测试中英文词汇汇总表)
      * [<a href="http://www.51testing.com/html/12/480312-814448.html" rel="nofollow">软件测试中一般术语的英文和缩写</a>](#软件测试中一般术语的英文和缩写)
   * [Resource](#resource)
      * [<a href="https://github.com/didi/rdebug">RDebug - Real Debugger (流量复制和回放框架)</a>](#rdebug---real-debugger-流量复制和回放框架)
