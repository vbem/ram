# 创建 RAM 用户 {#concept_gpm_ccf_xdb .concept}

在创建 RAM 用户前，确保您已完成[RAM 初始设置](cn.zh-CN/快速入门/RAM 初始设置.md)。

本文将指导您创建一个 RAM 用户，并根据用户的使用需求，分别为用户设置登录密码（如果该用户需要登录控制台），或 AccessKey（如果用户需要以程序方式调用云服务 API）。

## 创建 RAM 用户 {#section_qt4_dcf_xdb .section}

执行以下步骤创建 RAM 用户：

1.  在RAM控制台点击左侧导航栏中的**用户管理**。
2.  点击右上角**新建用户**，进入创建用户页面。
3.  输入用户信息后，点击**确认**。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/12340/3520_zh-CN.png "创建用户")


至此，您已完成 RAM 用户创建。

## 为用户设置登录密码 {#section_tt4_dcf_xdb .section}

对于已创建的 RAM 用户，如果该用户需要登录到控制台，则应为其配置登录密码。

## 操作步骤 {#section_ut4_dcf_xdb .section}

1.  在RAM控制台点击左侧导航栏中的**用户管理**。
2.  选择需要设置密码的用户（可通过**登录名** 进行搜索），并点击该用户名或其用户菜单下的**管理** 按钮，进入用户详情页。
3.  在**Web控制台登录管理**下，点击**启用控制台登录**。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/12340/6206_zh-CN.png "启用控制台登录")

4.  在弹窗中为用户设置初始密码，并可以指定用户登录时必须更换密码。

     ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/12340/3522_zh-CN.png "设置登录密码") 


至此，您已为 RAM 用户设置登录密码。

-   如需使用 RAM 子账号登录进行测试，请参照[RAM 用户登录控制台](cn.zh-CN/快速入门/RAM 用户登录控制台.md)。
-   如需对 RAM 子账号登录密码进行管理，请执行步骤 1~3，并在**Web控制台登录管理** 下，选择**重置密码**或者**关闭控制台登录**。

## 为用户创建AK {#section_zt4_dcf_xdb .section}

对于已创建的 RAM 用户，如果该用户需要以程序方式调用云服务 API，则应为其创建 AccessKey（AK）。

## 操作步骤 {#section_a54_dcf_xdb .section}

1.  在RAM控制台点击左侧导航栏中的**用户管理**。
2.  选择需要设置密码的用户（可通过**登录名**进行搜索），并点击该用户名或其用户菜单下的**管理**按钮，进入用户详情页。
3.  在**用户AccessKey**子页下，点击**创建AccessKey**。

     ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/12340/3523_zh-CN.png "创建AccessKey") 

4.  新建 Accesskey 成功后，点击保存**保存AK信息**。

    **说明：** 

    -   AccessKeySecret 只会在 AK 创建时提供查看或下载，为了安全考虑，后续不会提供AccessKeySecret 的再次查看或下载功能。

    -   如果 AK 丢失，您只能重新创建 AK。新创建的 AK 与原来的 AK 都是代表相同的用户身份，同一个 RAM 用户的不同 AK 在使用上是完全等效的。

    -   建议您为应用程序周期性更换 AK，避免因为 AK 泄露导致风险。


至此，您已为 RAM 用户创建 AccessKey。如需对用户的 AK 进行管理，请执行步骤 1~3，然后在用户AccessKey子页下，选择**禁用**或**删除**已创建的 AccessKey。

## 后续操作 {#section_e54_dcf_xdb .section}

对于已创建的 RAM 用户，在正常使用前，需要根据其职责对其进行访问资源授权。

-   给 RAM 用户授权，请参照 [为 RAM 用户授权](cn.zh-CN/快速入门/为 RAM 用户授权.md)。

-   创建粒度精细的自定义的授权策略，请参照[创建自定义授权策略（可选）](cn.zh-CN/快速入门/创建自定义授权策略（可选）.md)创建自定义授权策略。


