## 样本说明
  收集到12306泄漏数据共**131653**条，每条有**7**列数据，这七列数据分别为：
    - 姓名
    - 身份证号码
    - 手机号
    - 网站用户名
    - 网站绑定邮箱
    - 网站密码
    - 购票邮箱

## 密码分析

#### 密码长度分析

| 长度  | 人数  |  比例 | 备注                          | 
|-------|-------|-------|-------------------------------|
| -5    | 1     |  0%   | 网站注册密码最少6位,脏数据一条|
| 6     | 14732 | 11.19%|                               |
| 7     | 19857 | 15.08%|                               |
| 8     | 34715 | 26.37%|                               |
| 9     | 30737 | 23.25%|                               |
| 10    | 23857 | 18.12%|                               |
| 11    | 4496  | 3.42% |                               |
| 12    | 1984  | 1.51% |                               |
| 13    | 713   | 0.54% |                               |
| 14    | 403   | 0.31% |                               |
| 15    | 157   | 0.12% |                               |
| 16    | 1     |  0%   | 键盘弱密码                    |
| 17-   | 0     |  0%   | 没有17位以上密码              |
| Total | 131653|  100% | 全部统计                      |

- 密码长度在[6， 10]位之间有 **123898** 条数据，占比 **94.11%**

#### 密码类型分析

| 类型        |   数量   |  比例   |  备注|
|-------------|----------|---------|------|
| 纯数字      |   35572  |  27.02% |      |
| 纯小写字母  |   6947   |  5.28%  |      |
| 纯大写字母  |   62     |  0.05%  |      |
| 数字小写字母|   87664  |  66.59% |      |
| 数字大写字母|   490    |  0.37%  |      |
| 大小写字母  |   152    |  0.12%  |      |
| 常用字符混合|   755    |  0.57%  |      |
| Total       |   131642 |  99.99% |      |

真正的大小写字母、数字、特殊符号混合的密码只有116个，如果加上长度要求，则更少


#### 弱密码类型分析

###### 社工型弱密码
| 类型      | 数量  |  备注   |
|-----------|-------|---------|
| 手机号    | 602   | 正则匹配| 
| 生日      |       |         |
| 用户名    |       |         |
| qq        |       |         |

###### 顺序型弱密码
| 类型    |   数量   |  占比   |   备注 |
|---------|----------|---------|--------|
| 字母序  |          |         |        |
| 键盘序  |          |         |        |
| 英文单词|          |         |        |


## 邮箱分析

#### 邮箱后缀分布

| 后缀        |   数量   |  比例  |  备注  |
|-------------|----------|--------|--------|
| qq.com      |   73444  |  55.79%|        |
| 163.com     |   30448  |  23.13%|        |
| 126.com     |   11871  |  9.02% |        |
| sina.com    |   4900   |  3.72% |        |
| hotmail.com |   1966   |  1.49% |        |
| yahoo.com.cn|   1775   |  1.35% |        |
| vip.qq.com  |   1679   |  1.28% |        |
| gmail.com   |   1575   |  1.20% |        |
| sohu.com    |   1100   |  0.84% |        |
| yahoo.cn    |   544    |  0.41% |        |

  使用腾讯和网易邮箱的数据有 117442 条，占比89.21%


## 身份证分析

#### 样本说明
  - 数据中一部分使用的证件不是身份证，有台胞证、港澳通行证、护照。
  - 身份证有新旧身份证。
  - 新身份证倒数第二位为性别位

#### 性别分析
| 性别  |  数量  |  比率  | 备注 |
|-------|--------|--------|------|
| 男    |  121552|  92.33%|      |
| 女    |  9863  |  7.49% |      |

  男性占极大多数，原因可能是数据撞库自17173，男性玩家较多

#### 年龄分析
| 出身年份 | 数量 | 备注 |
|----------|------|------|
| 1989     | 15287|      |
| 1988     | 14894|      |
| 1987     | 13579|      |
| 1990     | 12974|      |
| 1986     | 11189|      |
| 1991     | 8478 |      |
| 1985     | 8372 |      |
| 1984     | 6681 |      |
| 1992     | 5676 |      |
| 1983     | 5629 |      |
| 总计     |102759|78.05%|

#### 出生月份分析
| 月份  |  数量  | 备注  |
|-------|--------|-------|
| 1     |  11223 |       |
| 2     |  10596 |       |
| 3     |  10380 |       |
| 4     |   9569 |       |
| 5     |   9897 |       |
| 6     |  10340 |       |
| 7     |  10536 |       |
| 8     |  11739 |       |
| 9     |  11262 |       |
| 10    |  13242 |       |
| 11    |  11620 |       |
| 12    |  11010 |       |
| 总计  |  131414| 99.82%|

#### 籍贯分析

| 省籍   |  人数   | 备注 |
|--------|---------|------|
| 湖北省 |  9683   |      |
| 江苏省 |  8914   |      |
| 浙江省 |  8770   |      |
| 四川省 |  8500   |      |
| 湖南省 |  8484   |      |
| 河南省 |  8015   |      |
| 山东省 |  6890   |      |
| 黑龙江 |  6688   |      |
| 福建省 |  5798   |      |
| 安徽省 |  5591   |      |

| 市籍          |    人数    |    备注         |
|---------------|------------|-----------------|
| 上海市 市辖区 |    3106    |                 |
| 浙江省 温州市 |    2443    |                 |
| 北京市 市辖区 |    2014    |                 |
| 湖北省 武汉市 |    1997    |                 |
| 福建省 福州市 |    1458    |17173成立于福州市|
| 黑龙江 哈尔滨 |    1368    |                 |
| 湖南省 衡阳市 |    1283    |                 |
| 四川省 成都市 |    1278    |                 |
| 江苏省 南京市 |    1172    |                 |
| 福建省 泉州市 |    1143    |                 |

