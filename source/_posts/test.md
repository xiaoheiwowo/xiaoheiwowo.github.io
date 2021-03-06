---
title: 软件测试
date: 2021-5-16
---

## 软件测试基础

- 测试定义
  - 通过人工或者自动的手段，对被测对象进行检测的活动，目的在于发现被测对象是否实现了用户的需求，或者弄清实际结果与预期目标的差异
  - 需要根据什么进行测试
    - 源代码
    - 用户手册
    - 配置数据
- 测试目的
  - 发现被测对象与用户需求之间的差异
  - 通过测试活动发现并解决缺陷，增加用户对被测对象的质量信心
  - 通过测试互动，获取被测对象的质量信息，为决策提供数据依据
  - 通过测试活动，预防缺陷，从降低项目或产品的风险
- 测试原则
  - 测试证明软件存在缺陷
  - 不可能执行穷尽测试
  - 测试应该尽早启动，尽早介入
  - 缺陷存在集群现象
  - 杀虫剂悖论
  - 不同的测试活动依赖不同的测试背景
  - 不存在缺陷的谬论



## 测试级别

- 单元测试
  - 针对被测系统最小的组成单元实施的测试活动，一般针对函数或者类，或者最小功能单元
- 集成测试
  - 针对组件/单元与组件/单元之间的接口实施的测试活动，验证接口设计是否与设计相符
  - 三种集成
    - 函数间集成
    - 模块间集成
    - 子系统间集成
- 系统测试
  - 讲通过集成测试的软件，部署在真实的用户环境执行测试
- 验收测试
  - 以用户为主的测试，验收组应该有项目组成员、用户代表组成
  - α测试
    - 由用户在开发环境执行的测试活动，开发者在测试人员身边，发现问题及时沟通解决
    - 在受控环境下执行测试
  - β测试
    - 开发者不再测试人员身边，发现问题有专人同意收集，再由研发人员进行修改
    - 再不受控环境下执行
  - UAT测试
    - 用于接受度测试 一般商业用户验证系统可用性进行的测试





## 系统测试类型

- 功能性测试
  - 在指定使用条件下，使用被测对象，验证其是否满足用于显性或隐性需求
  - 测试关注点
    - 是否有不正确或遗漏或多于的功能
    - 满足系统显性或隐性需求
    - 是否对输入输出做出了正确的响应，输出结果能否正确的显示
- 性能测试（借助压测工具）并发 响应时间等
  - 通过模拟被测对象运行业务压力或使用场景，验证被测对象是否满足预先设定的性能指标
  - 验证系统是否具有宣称的能力
  - 了解测试系统典型场景，并具有确定的性能目标
  - 要求在真实环境下实施
- 安全性测试
  - 测试被测对象的安全保护机制保护系统不受非法侵入，能够接受正确授权的操作
- 兼容性测试
  - 验证被测对象在不同的操作系统、硬件信息等环境下的运行情况



## 软件测试方法

- 黑盒测试
  - 不关注被测对象内部结构，仅从用于需求考虑，是否满足用户显性或隐性需求
- 白盒测试（结构测试，逻辑驱动测试）关注内部接口，结构
- 灰盒测试
  - 既关注被测对象的外部特性，又关注其内部设计
- 静态测试
  - 不执行被测对象程序，不运行被测对象的测试方法 （看代码，文档）
- 动态测试
  - 步骤
    - 阅读需求，编写用例
    - 评审
    - 搭建环境，执行应用
    - 进行测试
- 手工测试 
- 自动化测试 通过自动化测试工具或脚本自动完成测试
  - 功能 selenium
  - 性能 。。



## 软件质量



- 质量定义
  - 软件产品满足用户或规定显性或隐性需求的程度
  - 内部质量
  - 过程质量
  - 外部质量
  - 使用质量
- 质量特性（标准要求）
  - 功能性
    - 定义：软件在指定条件下使用时，满足用户明确和隐含需求的功能的能力
    - 适合性：软件为指定的任务和用户目标提供一组合适功能的能力
    - 准确性：软件提供具有所需精确度的正确或相符的结果或效果的能力
    - 互操作性：软件与一个或更多规定系统进行交互的能力
    - 保密安全性：软件保护信息和数据的能力，以使未授权的人员或系统不能阅读或修改这些信息和数据，而不拒绝授权人员或系统对他们的访问。
    - 功能性依从性：软件遵循与功能性相关的标准、约定或法规以及类似规定的能力。这些标准要考虑到国际标准、国家标准、行业标准、企业内部规范等。
  - 可靠性
    - 定义：软件为避免由软件中错误而导致失效的能力。
    - 成熟性：软件为避免由软件中错误而导致失效的能力。
    - 容错性：在软件出现故障或违反指定接口的情况下，软件维持规定的性能级别的能力。
    - 易恢复性：在失效发生的情况下，软件重建规定的性能级别并恢复受直接影响的数据的能力。
    - 可靠性依从性：软件遵循与可靠性相关的标准、约定或法规的能力。
  - 易用性：
    - 定义：在指定条件下使用时，软件被理解、学习、使用和吸引用户的能力。
    - 易理解性：软件使用户能理解软件是否合适，以及如何能将软件用于特定的任务和使用环境的能力。
    - 易学性：软件使用户能学习其应用的能力
    - 易操作性：软件使用户能操作和控制它的能力
    - 吸引性：软件吸引用户的能力
    - 易用性依从性：软件遵循各种标准法规预定的能力
  - 效率
    - 定义：在规定条件下，相对于所用资源的数量，软件可提供适当性能的能力
    - 时间特性：在规定条件下，相对于所用资源的数量，软件可提供适当性能的能力
    - 资源利用性：在规定条件下，软件执行其功能时，使用合适资源数量和类别的能力
    - 效率依从性：
  - 可移植
    - 定义：软件可被修改的能力。修改可能包括修正，改进或对软件对环境、需求和功能规格说明变化的适应。
    - 易分析性：软件诊断软件中的缺陷、失效原因或识别待修改部分的能力
    - 易改变性：软件使指定的修改可以被实现的能力。
    - 稳定性：软件避免由于软件修改而造成意外结果的能力。
    - 易测试性：软件使易修改软件能被确认的能力
    - 维护性依从性：标准法规
  - 可维护
    - 定义：软件从一种环境迁移到另外一种环境的能力。
    - 适应性：软件无需采用有别于为考虑软件的目的而准备的活动或手段，就可以适应不同的的指定环境的能力。
    - 易安装性：软件在指定环境中被安装的能力。
    - 共存性：软件在公共环境中通其分享公共资源的其他独立软件共存的能力。
    - 易替换性：软件在同样环境下，替代另一个相同用途的指定软件产品的能力。
    - 可移植性依从性：标准法规





## 系统测试流程（计划设计实现执行）

- 测试计划设计
  - 目标
  - 总体概述
    - 项目背景
    - 项目范围
  - 测试计划（管理层）
    - 测试资源需求
      - 软件资源
        - 操作系统 windows linux mac
        - 数据库 sqlserver mysql oracle 
        - web服务器 IIS Tomcat JBOSS ...
        - ！版本号
      - 硬件资源 服务器 手机 。。测试设备
      - 其他设备资源
      - 人员需求
    - 组织形式
    - 测试对象
    - 需求跟踪
    - 测试通过失败标准
    - 测试挂起恢复条件
    - 测试风险及预防
    - 测试任务安排
  - 应交付的测试工作产品
  - 资源分配
    - 培训需求
    - 测试工具开发
- 测试需求分析（测试团队）工具（QC 禅道）
  - 分析需求来源
    - 需求规格说明书
    - 开发需求
    - 继承性需求
    - 行业竞品分析
    - 经验库
  - 需求分类
    - 功能性需求
    - 性能需求
    - 外部接口需求
      - GUI
      - 外部应用程序接口需求
    - 也可以根据软件质量特性划分需求
      - 安全性
      - 效率
      - 可移植
      - 可维护
- 测试策略设计
- 测试规程设计
  - 测试需求变更控制流程
  - 测试用例变更控制流程
  - 测试环境搭建流程
  - 缺陷管理流程
- 测试用例设计
- 配置测试环境
  - 分平台：win linux unix
  - 分架构：j2ee .net lamp
  - 分web服务器：iis tomcat ...
  - 分数据库：
  - 自己注：移动平台 比如打包app
- 执行测试用例
  - 预测试阶段（冒烟测试）核心 重要 高风险功能快速测试 用例来源于高优先级的测试用例 预测试转系统测试评审
  - 系统测试
    - 经过预测试后，开展系统测试
    - 测试执行过程中发现缺陷，则需及时记录缺陷，根据部门或团队的缺陷管理流程进行缺陷提交。跟踪处理（最喜欢的提bug环节哈哈）
- 缺陷跟踪回归
- 测试报告输出
  - 测试日报
    - 方便测试工程师掌握测试进度和测试情况，用于调整下一天的工作计划
    - 测试工程师对被测对象每天给出评估结果，用于调整后续工作中的测试策略
    - 测试经理通过测试日报了解每个测试工程师的工作进度，把握测试整体进度，发现进度上的风险从而及时调整计划，人力资源
    - 不同测试组或测试工程师之间交流
  - 测试报告
    - 评估软件测试工程师当前被测对象的质量，并对下一阶段的测试工作给出建议
    - 测试经理通过测试报告了解被测试产品的质量情况、测试过程的质量
    - 软件开发项目经理通过软件测试报告了解开发产品的质量情况，并在下阶段的开发工作中采取应对措施。
    - 在测试报告中，测试工程师给出的产品质量评估可以作为软件产品是否商用发布的重要参考依据。
  - 测试报告模板
- 测试结束活动
  - 检查在测试过程中测试计划中定义的输出物
  - 缺陷管理是否完成，是否已经进入缺陷管理流程
  - 测试实施过程中产生的风险报告需要记录
  - 测试报告是否输出，相关的经验教训是否总结并分享
  - 是否需要移交测试对象



## 测试用例格式

- 用例编号
- 测试项
- 测试标题
- 用例属性
  - 功能测试
  - 性能测试
  - 兼容性测试
  - 安全测试
- 重要级别
  - 高：实现主体功能的用例
  - 中：主项流程经过备选流处理或者经过异常处理能够正确实现
  - 低：GUI 易用性表述 文字描述类
- 预置条件
- 测试输入：源数据
- 操作步骤：根据用户需求
- 预期输出：界面，功能
- 实际结果：

### 设计测试用例中的一些概念

- 等价类
  - 等价
    - 具有相同属性或方法的事务集合
    - 这个集合中某个个体所表现的特征与其他个体完全一致
    - 对于某个被测对象的测试输入而言，某个个体能够被接受或者被拒绝，则该个体所在集合中的任意个体都应该被接受或拒绝
  - 等价类划分
    - 有效等价类
      - 针对被测对象而言，合理的，有意义的，系统接受的输入
    - 无效等价类
      - 不合理 无意义 系统不接受的
  - 等价类划分规则
    - 如果需求规定了输入域的取值个数或确定了某个范围时，则可确定一个有效等价类和两个无效等价类（大于 小于）
    - 如果需求规定了某个输入域的集合，或者必须如何的情况下的，可确定一个有效和一个无效（）
    - 输入域规定真假值
    - 输入域规定一组值
    - 输入域规定某种规则（可以多个）可以确定一个有效等价类和若干无效等价类
  - 进行用例设计
    - 根据需求，划分有效及无效等价类，分别统一编号
    - 设计一个新的测试用例，使其尽可能覆盖所有尚未覆盖的有效等价类，直到所有等价类都被覆盖
    - 设计一个新的测试用例，使其仅覆盖一个无效等价类，直到所有无效等价类都被覆盖
  - 等价类四则运算法 （根据需求的规则设计有效和无效等价类）
    - 加：不考虑需求其他子项，细致分解当前测试点及详细需求，做累加
    - 减：根据业务规则减少，排除相关不可能出现的规则，减少不可能出现的组合
    - 乘：如果有效等价类中具有互斥条件的需求时，可进行相乘得到用例个数
    - 除：排除所有具有重复特性的等价类，尽可能做到有效等价类之间交集为空，无效等价类之间交集也为空，有效及无效等价类的并集为整个输入域
- 边界值
- 判定表
- 因果图
- 正交实验
- 状态迁移
- 流程分析
