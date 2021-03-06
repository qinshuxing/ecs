# 移除浮动IP<a name="ZH-CN_TOPIC_0065817719"></a>

## 功能介绍<a name="zh-cn_topic_0057973008_section9177509"></a>

从弹性云服务器上解绑浮动IP。

## 接口约束<a name="zh-cn_topic_0057973008_section5180770"></a>

-   该API准备废弃，从微版本2.44开始，调用该接口将报404错误。建议直接使用对应的网络服务接口["更新浮动IP"](https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333023.html)。

## URI<a name="zh-cn_topic_0057973008_section15488722"></a>

POST /v2/\{project\_id\}/servers/\{server\_id\}/action

POST /v2.1/\{project\_id\}/servers/\{server\_id\}/action

参数说明请参见[表1](#zh-cn_topic_0057973008_table32475667)。

**表 1**  参数说明

<a name="zh-cn_topic_0057973008_table32475667"></a>
<table><thead align="left"><tr id="zh-cn_topic_0057973008_row44937496"><th class="cellrowborder" valign="top" width="22.24%" id="mcps1.2.4.1.1"><p id="p5187119"><a name="p5187119"></a><a name="p5187119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.87%" id="mcps1.2.4.1.2"><p id="p17503500"><a name="p17503500"></a><a name="p17503500"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="55.88999999999999%" id="mcps1.2.4.1.3"><p id="p8497414"><a name="p8497414"></a><a name="p8497414"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0057973008_row1664874"><td class="cellrowborder" valign="top" width="22.24%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057973008_p637140"><a name="zh-cn_topic_0057973008_p637140"></a><a name="zh-cn_topic_0057973008_p637140"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.87%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057973008_p51608407"><a name="zh-cn_topic_0057973008_p51608407"></a><a name="zh-cn_topic_0057973008_p51608407"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="55.88999999999999%" headers="mcps1.2.4.1.3 "><p id="p37593705"><a name="p37593705"></a><a name="p37593705"></a>项目ID。</p>
<p id="p1180512217438"><a name="p1180512217438"></a><a name="p1180512217438"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0057973008_row41565035"><td class="cellrowborder" valign="top" width="22.24%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057973008_p11324657"><a name="zh-cn_topic_0057973008_p11324657"></a><a name="zh-cn_topic_0057973008_p11324657"></a>server_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.87%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057973008_p44882061"><a name="zh-cn_topic_0057973008_p44882061"></a><a name="zh-cn_topic_0057973008_p44882061"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="55.88999999999999%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057973008_p11568292"><a name="zh-cn_topic_0057973008_p11568292"></a><a name="zh-cn_topic_0057973008_p11568292"></a>云服务器ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0057973008_section16989244"></a>

**请求参数**

请求参数如[表2](#zh-cn_topic_0057973008_table20592177)所示。

**表 2**  请求参数

<a name="zh-cn_topic_0057973008_table20592177"></a>
<table><thead align="left"><tr id="zh-cn_topic_0057973008_row40662280"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0057973008_p5310363"><a name="zh-cn_topic_0057973008_p5310363"></a><a name="zh-cn_topic_0057973008_p5310363"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0057973008_p27486230"><a name="zh-cn_topic_0057973008_p27486230"></a><a name="zh-cn_topic_0057973008_p27486230"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.35%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0057973008_p11792162"><a name="zh-cn_topic_0057973008_p11792162"></a><a name="zh-cn_topic_0057973008_p11792162"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.650000000000006%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0057973008_p15641062"><a name="zh-cn_topic_0057973008_p15641062"></a><a name="zh-cn_topic_0057973008_p15641062"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0057973008_row58966539"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0057973008_p11560377"><a name="zh-cn_topic_0057973008_p11560377"></a><a name="zh-cn_topic_0057973008_p11560377"></a>removeFloatingIp</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0057973008_p63975319"><a name="zh-cn_topic_0057973008_p63975319"></a><a name="zh-cn_topic_0057973008_p63975319"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0057973008_p14618317"><a name="zh-cn_topic_0057973008_p14618317"></a><a name="zh-cn_topic_0057973008_p14618317"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0057973008_p43233028"><a name="zh-cn_topic_0057973008_p43233028"></a><a name="zh-cn_topic_0057973008_p43233028"></a>弹性云服务器解绑浮动IP</p>
</td>
</tr>
</tbody>
</table>

**表 3**  removeFloatingIp参数信息

<a name="zh-cn_topic_0057973008_table12214371"></a>
<table><thead align="left"><tr id="zh-cn_topic_0057973008_row11201709"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p61001030132313"><a name="p61001030132313"></a><a name="p61001030132313"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p4100163062315"><a name="p4100163062315"></a><a name="p4100163062315"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.35%" id="mcps1.2.5.1.3"><p id="p81003304234"><a name="p81003304234"></a><a name="p81003304234"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.650000000000006%" id="mcps1.2.5.1.4"><p id="p71001930132315"><a name="p71001930132315"></a><a name="p71001930132315"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0057973008_row48978777"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0057973008_p7857996"><a name="zh-cn_topic_0057973008_p7857996"></a><a name="zh-cn_topic_0057973008_p7857996"></a>address</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0057973008_p32517948"><a name="zh-cn_topic_0057973008_p32517948"></a><a name="zh-cn_topic_0057973008_p32517948"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0057973008_p16708112"><a name="zh-cn_topic_0057973008_p16708112"></a><a name="zh-cn_topic_0057973008_p16708112"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0057973008_p11179825"><a name="zh-cn_topic_0057973008_p11179825"></a><a name="zh-cn_topic_0057973008_p11179825"></a>浮动IP的IP地址</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0057973008_section18685471"></a>

不涉及

## 示例<a name="zh-cn_topic_0057973008_section33951514"></a>

-   请求示例

    ```
    POST /v2/9c53a566cb3443ab910cf0daebca90c4/servers/47e9be4e-a7b9-471f-92d9-ffc83814e07a/action
    POST /v2.1/9c53a566cb3443ab910cf0daebca90c4/servers/47e9be4e-a7b9-471f-92d9-ffc83814e07a/action
    {
       "removeFloatingIp" : {
            "address" : "10.144.2.1"
        }
    }
    ```

-   响应示例

    不涉及


## 返回值<a name="zh-cn_topic_0057973008_zh-cn_topic_0020212692_section22960139"></a>

请参考[通用请求返回值](通用请求返回值.md)。

