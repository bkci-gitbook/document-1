# 删除流水线编排

### 请求方法/请求路径

#### DELETE  /ms/openapi/api/apigw/v3/projects/{projectId}/pipelines/{pipelineId}

### 资源描述

#### 删除流水线编排

### 输入参数说明

#### Query参数

| 参数名称 | 参数类型 | 必须 | 参数说明 | 默认值 |
| :--- | :--- | :--- | :--- | :--- |
| channelCode | string | 否 | 渠道号，默认为BS |  |

#### Path参数

| 参数名称 | 参数类型 | 必须 | 参数说明 | 默认值 |
| :--- | :--- | :--- | :--- | :--- |
| projectId | string | 是 | 项目ID |  |
| pipelineId | string | 是 | 流水线ID |  |

#### 响应

| HTTP代码 | 说明 | 参数类型 |
| :--- | :--- | :--- |
| 200 | successful operation | [数据返回包装模型Boolean](delete-the-pipeline-orchestration.md) |

#### 请求样例

```javascript
curl -X DELETE '[请替换为API地址栏请求地址]?channelCode={channelCode}'
```

#### HEADER样例

```javascript
accept: application/json
Content-Type: application/json
```

### 返回样例-200

```javascript
{
  "data" : true,
  "message" : "String",
  "status" : 0
}
```

## 数据返回包装模型Boolean

| 参数名称 | 参数类型 | 必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| data | boolean | 否 | 数据 |
| message | string | 否 | 错误信息 |
| status | integer | 是 | 状态码 |

