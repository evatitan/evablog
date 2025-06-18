---
title: Coding Terminology for web developers
description: "Coding Terminology "
date: 2025-05-10
image: "/images/posts/coding-terms.png"
categories: ["programming"]
authors: ["Evatitan"]
tags: ["terms"]
draft: false
---

For any of non-native English-speakers programmers, seeing coding terms for the first time can be intimidating. This is not only because they are technical terms but also because they can seem a little abstract at first. There are so many of them! So I created this coding terms outline for myself and others coders.

# Coding Terminology

## JavaScript terms 

| Term  | Definition  | Chinese |
|-------|-------------|---------|
| Event delegation      | A technique of handling events at a higher level in the DOM rather than on individual elements            | 事件委托，在父元素上处理子元素事件         |
| IIFE (Immediately Invoked Function Expression)       | A function that runs as soon as it is defined            | 立即执行函数表达式，定义后立即运行的函数         |
| Temporal Dead Zone      | The period between entering scope and variable declaration where variables can not be accessed             |  暂时性死区，变量声明前不可访问的区域        |
| Call Stack       | The mechanism for keep track of function calls in JS            | 调用栈，跟踪函数调用的机制        |
| Microtask | A type of task that executes after the currently executing script and before rendering or others tasks | 微任务，紧接当前脚本后执行的任务  |
| Macrotask | A type of task executes after Microtask, such as setTimeout or setInterval | 宏任务，如 setTimeout/setInterval 等  |
| Iterator  |An object that defines a sequence and potentially a return value upon its completion.  |迭代器，定义序列及返回值的对象  |
| Async Iterator      | An iterator that returns Promises, allowing for asynchronous iteration.     | 异步迭代器，返回 Promise 的迭代器           |
| Module Resolution   | The process by which JavaScript determines what code to load for an import or require. | 模块解析，确定导入/require 加载内容的过程   |
| Dynamic Import      | Importing modules dynamically at runtime using `import()`.                  | 动态导入，运行时使用 import() 加载模块       |
| Call Apply Bind     | Methods for controlling function invocation and context (`this`).           | call/apply/bind，控制函数调用和 this 的方法  |
| Context (this)      | The value of `this` keyword in different execution contexts.                | 上下文（this），不同执行环境下的 this 值     |
| Optional Chaining   | A syntax (`?.`) for accessing deeply nested properties safely.              | 可选链，安全访问深层属性的语法               |
| Nullish Coalescing  | A syntax (`??`) for providing a default value when the left operand is null or undefined. | 空值合并运算符，左侧为 null/undefined 时提供默认值 |
| BigInt              | A built-in object for representing integers with arbitrary precision.        | BigInt，表示任意精度整数的内置对象           |
| Intl API            | JavaScript Internationalization API for formatting dates, numbers, etc.      | Intl API，国际化相关的内置 API               |
| Hot Reload          | Automatically reloading code changes in a running application without a full restart. | 热重载，代码变更自动刷新                    |
| Code Splitting      | Breaking up code into smaller chunks that can be loaded on demand.           | 代码分割，按需加载代码块                     |
| Lazy Loading        | Loading resources only when they are needed to improve performance.           | 懒加载，仅在需要时加载资源                   |
| SSR Hydration       | The process of attaching event listeners to server-rendered HTML on the client. | SSR 水合，将事件监听器附加到服务端渲染 HTML  |
| Static Site Generation (SSG) | Generating HTML pages at build time instead of on each request.     | 静态站点生成，构建时生成 HTML 页面           |
| Universal/Isomorphic JS | JavaScript code that runs both on the client and the server.             | 通用/同构 JS，前后端均可运行的 JS            |
| Middleware Stack    | A sequence of middleware functions that process requests/responses in web frameworks. | 中间件栈，依次处理请求/响应的中间件函数      |
| Dependency Graph    | A representation of how modules or components depend on each other.          | 依赖图，模块或组件之间依赖关系的表示         |
| Dependency Injection| A design pattern for providing dependencies to objects or functions.          | 依赖注入，向对象或函数提供依赖的设计模式     |
| Message Queue       | A system for exchanging messages between processes or services asynchronously. | 消息队列，异步交换消息的系统                 |
| Pub/Sub (Publish/Subscribe) | A messaging pattern where senders (publishers) do not program messages to be sent directly to receivers (subscribers). | 发布/订阅，发送者与接收者解耦的消息模式      |
| Middleware          | Functions that process requests and responses in web frameworks.              | 中间件，处理请求和响应的函数                 |
| Rollback            | Reverting to a previous stable version after a failed deployment.             | 回滚，部署失败后恢复到稳定版本               |
| API Versioning      | Managing changes to an API by creating multiple versions.                     | API 版本管理，通过多个版本管理 API 变更       |
| Shadow Deployment   | Deploying a new version of an application alongside the old one to test in production without affecting users. | 影子部署，与旧版本并行测试新版本             |
| Sticky Session      | Ensuring a user's requests are always routed to the same server in a load-balanced environment. | 粘性会话，负载均衡环境下请求总路由到同一服务器 |
| Monitoring          | Continuously observing a system’s health and performance.                     | 监控，持续观察系统健康和性能                 |
| Alerting            | Notifying operators or systems when certain conditions are met.               | 告警，条件满足时通知运维或系统               |
| Log Aggregation     | Collecting and centralizing logs from multiple sources for analysis.          | 日志聚合，集中收集和分析日志                 |
| Metrics             | Quantitative measurements used to assess system performance or health.        | 指标，衡量系统性能或健康的量化数据           |
| SLA (Service Level Agreement) | A contract that defines the expected level of service between a provider and a customer. | 服务级别协议，定义服务期望水平的合同         |
| SLO (Service Level Objective) | A specific measurable characteristic of the SLA, such as uptime or response time. | 服务级别目标，SLA 的具体可衡量特性           |
| SLI (Service Level Indicator) | A metric used to measure compliance with an SLO.                     | 服务级别指标，衡量 SLO 达成度的指标          |
| Non-blocking        | Operations that do not block program execution while waiting for tasks to complete. | 非阻塞，等待任务时不会阻塞程序执行         |
| Single Main Thread  | A program architecture where one main thread handles all tasks (common in JavaScript). | 单主线程，所有任务由一个主线程处理         |
| Polyfill            | Code that implements a feature on web browsers that do not support it natively. | Polyfill，为旧浏览器实现新特性的代码        |
| Transpiler          | A tool that converts code from one language or version to another.         | 转译器，将代码转换为另一种语言或版本         |
| Source Map          | A file that maps compiled code back to its original source code.           | Source Map，映射编译后代码到源代码的文件     |
| Tree Shaking        | A process of removing unused code during the build process.                | Tree Shaking，构建时移除未使用代码           |
| Set                 | A collection of unique values.                                              | Set，唯一值的集合                           |
| Map                 | A collection of key-value pairs with keys of any type.                       | Map，任意类型键的键值对集合                  |


<details>

<summary>React terms</summary>

| Term                        | Definition                                                                 | 中文解释                                   |
|-----------------------------|----------------------------------------------------------------------------|--------------------------------------------|
| Higher-order Component (HOC)| A function in React that takes a component and returns a new component with added functionality. | 高阶组件，增强组件功能的函数         |
| Lift State Up               | Moving shared state to a common ancestor component in React to manage data flow. | 状态提升，提升到共同父组件管理数据     |
| JSX                         | A syntax extension for JavaScript that looks similar to XML/HTML and is used with React to describe UI. | JSX，React 用于描述界面的语法扩展      |
| Props                       | Inputs to a React component, passed in as attributes.                        | Props，传递给组件的输入属性                |
| State                       | Data managed within a React component that can change over time.              | State，组件内部可变的数据                  |
| useState                    | A React Hook for adding state to functional components.                      | useState，给函数组件添加状态的 Hook         |
| useEffect                   | A React Hook for performing side effects in functional components.            | useEffect，处理副作用的 Hook                |
| useContext                  | A React Hook for accessing context values in functional components.           | useContext，访问上下文的 Hook               |
| useRef                      | A React Hook for persisting values across renders without causing re-renders. | useRef，跨渲染持久化值的 Hook               |
| useMemo                     | A React Hook for memoizing expensive calculations.                           | useMemo，缓存计算结果的 Hook                |
| useCallback                 | A React Hook for memoizing callback functions.                               | useCallback，缓存回调函数的 Hook            |
| Context                     | A way to pass data through the component tree without having to pass props down manually at every level. | Context，无需逐层传递 props 的数据共享方式   |
| Component                   | A reusable piece of UI in React, either a function or class.                  | 组件，React 中可复用的 UI 单元              |
| Controlled Component        | A component whose form data is handled by React state.                        | 受控组件，表单数据由 React 状态管理         |
| Uncontrolled Component      | A component that manages its own state internally via the DOM.                | 非受控组件，表单数据由 DOM 自己管理          |
| Fragment                    | A way to group multiple elements without adding extra nodes to the DOM.       | Fragment，分组多个元素但不增加 DOM 节点      |
| Portal                      | Rendering a child into a DOM node outside the parent component hierarchy.     | Portal，将子元素渲染到父组件层级外的 DOM 节点|
| Error Boundary              | A React component that catches JavaScript errors anywhere in its child component tree. | 错误边界，捕获子组件树错误的组件           |
| Reconciliation              | The process React uses to update the DOM efficiently.                         | 协调，React 高效更新 DOM 的过程             |
| Virtual DOM                 | An in-memory representation of the real DOM used by React for efficient updates. | 虚拟 DOM，React 用于高效更新的内存 DOM      |
| Key                         | A special string attribute used to identify elements in a list.               | Key，列表元素唯一标识符                     |
| Prop Drilling               | Passing data through many nested components via props.                        | Prop Drilling，通过多层组件传递 props        |
| Render Props                | A technique for sharing code between React components using a prop whose value is a function. | Render Props，通过函数 prop 共享代码         |
| PureComponent               | A React component that only re-renders when its props or state change.        | PureComponent，仅在 props 或 state 变化时重新渲染的组件 |
| Memoization                 | Optimization technique to avoid unnecessary renders by caching results.        | 记忆化，缓存结果以避免不必要的渲染           |
| React Router                | A library for handling routing in React applications.                         | React Router，React 应用的路由库             |
| Redux                       | A state management library often used with React.                             | Redux，常与 React 配合使用的状态管理库       |
| React Fiber                 | The new reconciliation engine in React 16+ for incremental rendering.          | React Fiber，React 16+ 的新协调引擎          |
| Synthetic Event             | A cross-browser wrapper around the browser’s native event.                     | 合成事件，跨浏览器的事件封装                 |
| StrictMode                  | A tool for highlighting potential problems in an application.                   | StrictMode，突出潜在问题的工具               |

</details>

<details>

<summary>Browser terms</summary>

| Term                        | Definition                                                                 | 中文解释                                   |
|-----------------------------|----------------------------------------------------------------------------|--------------------------------------------|
| SSR Hydration               | The process of attaching event listeners to server-rendered HTML on the client. | SSR 水合，将事件监听器附加到服务端渲染 HTML  |
| Static Site Generation (SSG)| Generating HTML pages at build time instead of on each request.             | 静态站点生成，构建时生成 HTML 页面           |
| Universal/Isomorphic JS     | JavaScript code that runs both on the client and the server.                | 通用/同构 JS，前后端均可运行的 JS            |
| Search Engine Optimization (SEO) | Techniques to improve a website’s visibility in search engine results. | 搜索引擎优化，提升网站在搜索引擎中的可见性   |
| Cross-Site Scripting (XSS)  | A security vulnerability allowing attackers to inject malicious scripts into web pages. | 跨站脚本攻击，允许攻击者注入恶意脚本         |


</details>


<details>

<summary>Database terms</summary>

| Term                        | Definition                                                                 | 中文解释                                   |
|-----------------------------|----------------------------------------------------------------------------|--------------------------------------------|
| Data-intensive              | Applications that process or handle large volumes of data.                 | 数据密集型，处理大量数据的应用               |
| Sharding                    | Splitting a database into smaller, faster, more easily managed parts called shards. | 分片，将数据库拆分为更小的部分              |
| Consistent Hashing          | A technique to distribute data across a cluster to minimize reorganization. | 一致性哈希，分布式数据分配技术              |
| Time Series Database        | A database optimized for time-stamped or time series data.                 | 时序数据库，优化存储时间序列数据            |
| Graph Database              | A database that uses graph structures for semantic queries.                | 图数据库，使用图结构进行查询                |
| Data Lake                   | A centralized repository for storing all structured and unstructured data at any scale. | 数据湖，集中存储结构化和非结构化数据        |
| Data Warehouse              | A system used for reporting and data analysis, storing structured data from multiple sources. | 数据仓库，用于分析和报告的结构化数据存储    |
| ETL                         | Extract, Transform, Load – a process in data warehousing.                  | ETL，数据抽取、转换和加载过程               |
| Migration                   | The process of changing a database schema over time.                       | 迁移，数据库结构变更过程                    |
| ACID                        | A set of properties guaranteeing reliable database transactions.            | ACID，保证数据库事务可靠性的属性            |
| Index                       | A database structure that improves the speed of data retrieval.             | 索引，提高数据库查询速度                    |
| Query                       | A request for data or information from a database.                          | 查询，向数据库请求数据                      |

</details>


<details>

<summary>Git terms</summary>

| Term                | Definition                                                                 | 中文解释                                   |
|---------------------|----------------------------------------------------------------------------|--------------------------------------------|
| Fork                | Creating a personal copy of someone else's repository.                     | 派生，复制他人仓库到自己账户                |
| Pull Request (PR)   | A request to merge changes from one branch or fork into another.           | 拉取请求，合并分支或派生仓库的更改           |
| Push                | Uploading local commits to a remote repository.                            | 推送，将本地提交上传到远程仓库               |
| Pull                | Fetching and integrating changes from a remote repository.                  | 拉取，从远程仓库获取并合并更改               |
| Fetch               | Downloading new data from a remote repository without integrating it.      | 获取，仅下载远程仓库的新数据                 |
| Stash               | Temporarily saving changes that are not ready to be committed.             | 贮藏，临时保存未提交的更改                   |
| Tag                 | Marking a specific commit as important (e.g., for releases).               | 标签，给 Docker 镜像打的版本标记            |
| Conflict            | A situation where changes from different sources cannot be automatically merged. | 冲突，不同更改无法自动合并               |
| .gitignore          | A file specifying which files and directories to ignore in a repository.   | .gitignore，指定仓库忽略的文件和目录         |
| Blame               | Showing who last modified each line of a file.                             | 追溯，显示每行代码的最后修改者               |
| Cherry-pick         | Applying a specific commit from one branch onto another branch.            | 拣选，将某个提交应用到另一个分支             |
| Revert              | Creating a new commit that undoes the changes of a previous commit.        | 撤销，生成新提交以还原先前更改               |
| Reset               | Moving the current branch to a specific commit, optionally modifying the index and working directory. | 重置，将分支指向特定提交                   |
| HEAD                | The current commit your working directory is based on.                     | HEAD，当前工作目录所基于的提交               |
| Upstream            | The main repository or branch that your branch tracks.                     | 上游，分支所跟踪的主仓库或主分支             |
| Detached HEAD       | A state where HEAD points directly to a commit instead of a branch.        | 游离 HEAD，HEAD 直接指向提交而非分支         |
| Fast-forward        | A type of merge that moves the branch pointer forward without creating a merge commit. | 快进合并，不产生合并提交的合并方式      |
| Submodule           | A repository embedded inside another repository.                            | 子模块，嵌套在另一个仓库中的仓库             |
| Reflog              | A log of where your HEAD and branch references have been.                  | Reflog，HEAD 和分支引用的历史记录            |

</details>



<details>

<summary>Docker terms</summary>


| Term                | Definition                                                                 | 中文解释                                   |
|---------------------|----------------------------------------------------------------------------|--------------------------------------------|
| Docker              | A platform for developing, shipping, and running applications in containers.| Docker，容器化平台                          |
| Container           | A lightweight, standalone, executable package that includes everything needed to run a piece of software. | 容器，包含运行软件所需全部内容的轻量包 |
| Dockerfile          | A text file with instructions to build a Docker image.                      | Dockerfile，构建镜像的指令文件              |
| Image               | A read-only template used to create containers.                             | 镜像，用于创建容器的只读模板                |
| Registry            | A storage and distribution system for Docker images (e.g., Docker Hub).     | 镜像仓库，存储和分发 Docker 镜像的系统      |
| Docker Hub          | The default public registry for Docker images.                              | Docker Hub，默认的公共镜像仓库              |
| Build               | The process of creating a Docker image from a Dockerfile.                   | 构建，从 Dockerfile 创建镜像的过程           |
| Pull                | Downloading a Docker image from a registry.                                 | 拉取，从仓库下载 Docker 镜像                |
| Push                | Uploading a Docker image to a registry.                                     | 推送，将 Docker 镜像上传到仓库              |
| Run                 | Creating and starting a new container from an image.                        | 运行，从镜像创建并启动新容器                |
| Volume              | A persistent storage mechanism for Docker containers.                       | 卷，Docker 容器的数据持久化机制             |
| Network             | A way for Docker containers to communicate with each other and the outside world. | 网络，容器间及与外部通信的方式         |
| Bind Mount          | Mounting a file or directory from the host into a container.                | 绑定挂载，将主机文件或目录挂载到容器        |
| Port Mapping        | Exposing container ports to the host machine.                               | 端口映射，将容器端口暴露给主机              |
| Compose             | A tool for defining and running multi-container Docker applications.         | Compose，定义和运行多容器应用的工具         |
| docker-compose.yml  | The configuration file for Docker Compose.                                  | docker-compose.yml，Compose 配置文件        |
| Swarm               | Docker's native clustering and orchestration solution.                      | Swarm，Docker 原生集群和编排方案            |
| Orchestration       | Automated management of containerized applications (e.g., scaling, failover).| 编排，自动管理容器应用（如扩缩容、故障转移）|
| ENTRYPOINT          | The command that is always executed when a container starts.                 | ENTRYPOINT，容器启动时始终执行的命令        |
| CMD                 | The default command to run when a container starts, can be overridden.       | CMD，容器启动时的默认命令，可被覆盖         |
| Layer               | Each instruction in a Dockerfile creates a new layer in the image.           | 层，Dockerfile 每条指令生成的镜像层         |
| Tag                 | A label applied to a Docker image for versioning.                            | 标签，给 Docker 镜像打的版本标记            |
| Healthcheck         | A command in Dockerfile to check container health.                           | 健康检查，检测容器健康状态的命令            |
| ENTRYPOINT vs CMD   | ENTRYPOINT is always executed; CMD provides default arguments for ENTRYPOINT.| ENTRYPOINT 总是执行，CMD 提供默认参数        |


</details>


<details>

<summary>Operating System terms</summary>

| Term        | Definition                                               | 中文解释                   |
|-------------|----------------------------------------------------------|----------------------------|
| Operating System (OS) | System software that manages hardware and software resources. | 操作系统，管理硬件和软件资源的系统 |
| Windows     | A widely used operating system developed by Microsoft.   | Windows，微软开发的操作系统 |
| Linux       | An open-source, Unix-like operating system.              | Linux，开源类 Unix 操作系统 |
| macOS       | The operating system developed by Apple for Mac computers.| macOS，苹果公司为 Mac 开发的操作系统 |
| Kernel      | The core part of an operating system, managing resources and communication between hardware and software. | 内核，操作系统的核心部分，管理资源和软硬件通信 |
| Shell       | A user interface for access to an operating system's services. | Shell，操作系统的命令行界面 |
| File System | The method and data structure that an OS uses to control how data is stored and retrieved. | 文件系统，操作系统用于管理数据存储和检索的方法和结构 |
| Process     | An instance of a running program.                        | 进程，正在运行的程序实例    |
| Thread      | The smallest unit of processing that can be scheduled by an OS. | 线程，操作系统可调度的最小处理单元 |
| Bash        | A popular Unix shell and command language.               | Bash，流行的 Unix Shell 和命令语言 |
| Command Line| A text-based interface for interacting with the OS.      | 命令行，与操作系统交互的文本界面 |

</details>



<details>

<summary>Advanced IT Terms</summary>

| Term                | Definition                                                                 | 中文解释                                   |
|---------------------|----------------------------------------------------------------------------|--------------------------------------------|
| CAP Theorem         | States that a distributed system can only guarantee two of Consistency, Availability, Partition tolerance. | CAP 定理，分布式系统一致性、可用性、分区容忍性三选二 |
| Sharding            | Splitting a database into smaller, faster, more easily managed parts called shards. | 分片，将数据库拆分为更小的部分              |
| Consistent Hashing  | A technique to distribute data across a cluster to minimize reorganization. | 一致性哈希，分布式数据分配技术              |
| Distributed Lock    | A mechanism to synchronize access to resources across multiple systems.     | 分布式锁，跨系统同步资源访问的机制           |
| Leader Election     | A process in distributed systems to designate a single node as the organizer. | 选主，分布式系统中选出唯一主节点            |
| Raft                | A consensus algorithm for managing a replicated log.                       | Raft，共识算法，用于管理复制日志             |
| Paxos               | A family of protocols for solving consensus in a network of unreliable processors. | Paxos，分布式一致性协议                  |
| Saga Pattern        | A pattern for managing distributed transactions using a sequence of local transactions. | Saga 模式，分布式事务管理模式             |
| Immutable Infrastructure | Infrastructure that is never modified after deployment.                | 不可变基础设施，部署后不再修改的基础设施     |
| Serverless          | A cloud-computing model where the cloud provider runs the server, and dynamically manages the allocation of machine resources. | 无服务器架构，云平台自动管理资源            |
| Edge Computing      | Processing data near the source of data generation rather than in a centralized data center. | 边缘计算，在数据源附近处理数据              |
| Data Lake           | A centralized repository for storing all structured and unstructured data at any scale. | 数据湖，集中存储结构化和非结构化数据        |
| Data Warehouse      | A system used for reporting and data analysis, storing structured data from multiple sources. | 数据仓库，用于分析和报告的结构化数据存储    |
| ETL                 | Extract, Transform, Load – a process in data warehousing.                   | ETL，数据抽取、转换和加载过程               |
| Data Pipeline       | A set of processes that move data from one system to another, often transforming it along the way. | 数据管道，数据流转和处理流程               |
| Container Orchestration | Automated management of containerized applications (e.g., Kubernetes).  | 容器编排，自动管理容器应用（如 Kubernetes）  |
| Kubernetes          | An open-source system for automating deployment, scaling, and management of containerized applications. | Kubernetes，容器编排系统                   |
| Service Discovery   | Automatically detecting devices and services on a network.                  | 服务发现，自动检测网络中的服务               |
| API Rate Limiting   | Restricting the number of API requests a client can make in a given time.   | API 限流，限制客户端请求频率                 |
| WebAssembly (WASM)  | A binary instruction format for a stack-based virtual machine, enabling high-performance apps on the web. | WebAssembly，Web 高性能二进制格式           |
| Progressive Web App (PWA) | Web apps that use modern web capabilities to deliver an app-like experience. | 渐进式 Web 应用，具备原生体验的网页应用    |
| Content Security Policy (CSP) | A security standard to prevent cross-site scripting and other attacks. | 内容安全策略，防止 XSS 等攻击              |
| OAuth2.0            | An authorization framework enabling third-party applications to obtain limited access to user accounts. | OAuth2.0，第三方授权框架                   |
| OpenID Connect      | An authentication layer on top of OAuth 2.0.                                | OpenID Connect，基于 OAuth2.0 的认证层      |
| SSO (Single Sign-On)| A session/user authentication process that permits a user to use one set of login credentials for multiple applications. | 单点登录，多个应用共用一套登录凭证         |
| RBAC (Role-Based Access Control) | Restricting system access to authorized users based on roles.     | 基于角色的访问控制，根据角色限制访问        |
| DDoS (Distributed Denial of Service) | An attack where multiple systems flood the bandwidth or resources of a targeted system. | 分布式拒绝服务攻击，多系统联合攻击目标      |
| CDN Edge Node       | A server in a CDN network that caches content closer to users.               | CDN 边缘节点，靠近用户的缓存服务器           |
| Hybrid Cloud        | A computing environment that uses a mix of on-premises, private cloud and public cloud services. | 混合云，结合本地和云服务的环境             |
| Multi-Cloud         | The use of multiple cloud computing services in a single architecture.        | 多云，单一架构中使用多个云服务              |
| Immutable Data Structure | Data structures that cannot be changed after creation.                   | 不可变数据结构，创建后不可更改的数据结构     |
| Eventual Consistency | A consistency model used in distributed computing to achieve high availability. | 最终一致性，分布式系统中的一致性模型        |
| Time Series Database | A database optimized for time-stamped or time series data.                   | 时序数据库，优化存储时间序列数据            |
| Graph Database      | A database that uses graph structures for semantic queries.                   | 图数据库，使用图结构进行查询                |
| Blockchain          | A distributed ledger technology for securely recording transactions.           | 区块链，分布式账本技术                      |
| Quantum Computing   | Computing using quantum-mechanical phenomena, such as superposition and entanglement. | 量子计算，利用量子力学现象的计算方式      |
| Homomorphic Encryption | Encryption that allows computation on ciphertexts, generating an encrypted result. | 同态加密，可在密文上直接计算                |
| Federated Learning  | A machine learning technique that trains an algorithm across multiple decentralized devices. | 联邦学习，分布式设备协同训练算法           |
| A/B Testing         | Comparing two versions of a web page or app to see which performs better.      | A/B 测试，对比两种版本的效果                |
| Feature Flag        | A technique to enable or disable features without deploying new code.          | 功能开关，不用重新部署即可控制功能           |
| Blue/Green Deployment | A release management strategy that reduces downtime and risk by running two identical production environments. | 蓝绿部署，两个环境切换发布                  |
| Chaos Monkey        | A tool that randomly disables production instances to test system resilience.   | 混沌猴，随机破坏实例以测试系统韧性           |
| Circuit Breaker Pattern | A design pattern to prevent repeated failures in distributed systems.      | 断路器模式，防止分布式系统反复故障           |
| Service Mesh        | A dedicated infrastructure layer for handling service-to-service communication. | 服务网格，服务间通信的基础设施层           |
| Sidecar Pattern     | Deploying supporting components of an application as a separate process or container. | Sidecar 模式，辅助组件独立部署              |
| Zero Trust Security | Security model that assumes no implicit trust, verifying everything.        | 零信任安全，默认不信任任何访问              |
| Observability Pipeline | The tooling and processes for collecting, processing, and analyzing logs, metrics, and traces. | 可观测性管道，收集和分析日志、指标、追踪的流程 |
| Tracing             | Tracking the flow of requests through distributed systems.                  | 链路追踪，跟踪分布式系统中的请求流           |
| Monitoring          | Continuously observing a system’s health and performance.                   | 监控，持续观察系统健康和性能                 |
| Alerting            | Notifying operators or systems when certain conditions are met.             | 告警，条件满足时通知运维或系统               |
| Log Aggregation     | Collecting and centralizing logs from multiple sources for analysis.        | 日志聚合，集中收集和分析日志                 |
| Metrics             | Quantitative measurements used to assess system performance or health.      | 指标，衡量系统性能或健康的量化数据           |
| SLA (Service Level Agreement) | A contract that defines the expected level of service between a provider and a customer. | 服务级别协议，定义服务期望水平的合同         |
| SLO (Service Level Objective) | A specific measurable characteristic of the SLA, such as uptime or response time. | 服务级别目标，SLA 的具体可衡量特性           |
| SLI (Service Level Indicator) | A metric used to measure compliance with an SLO.                   | 服务级别指标，衡量 SLO 达成度的指标          |
| Rollback            | Reverting to a previous stable version after a failed deployment.           | 回滚，部署失败后恢复到稳定版本               |
| Feature Toggle/Flag | A technique to enable or disable features without deploying new code.       | 功能开关，不用重新部署即可控制功能           |
| Canary Deployment   | Gradually rolling out a new software version to a small subset of users before a full rollout. | 金丝雀部署，逐步发布新版本         |
| Blue/Green Deployment | A release management strategy that reduces downtime and risk by running two identical production environments. | 蓝绿部署，两个环境切换发布         |
| Shadow Deployment   | Deploying a new version of an application alongside the old one to test in production without affecting users. | 影子部署，与旧版本并行测试新版本    |
| Shadow Traffic      | Sending a copy of production traffic to a new system for testing without impacting users. | 影子流量，生产流量副本用于测试      |
| Sticky Session      | A method to ensure a user's requests are always routed to the same server in a load-balanced environment. | 粘性会话，负载均衡环境下请求总路由到同一服务器 |
| Service Registry    | A database or directory of available services in a microservices architecture. | 服务注册表，微服务架构中的服务目录  |
| Data-intensive      | Applications that process or handle large volumes of data.                  | 数据密集型，处理大量数据的应用               |
| Cloud-native Application | Apps designed to run in cloud environments, leveraging scalability and resilience features. | 云原生应用，专为云环境设计的应用            |
| Bootstrap Abstraction | Extracting repeated setup/config logic into reusable layers to simplify code and improve reuse. | 启动抽象，提取重复配置逻辑以简化和复用代码   |
| I/O Framework       | Tools/libraries for handling input/output (e.g., files, network, user input). | I/O 框架，处理输入输出的工具或库            |
| Event-driven Programming | Programming paradigm where events trigger actions via listeners and emitters, often for async tasks. | 事件驱动编程，事件触发动作的编程范式         |

</details>