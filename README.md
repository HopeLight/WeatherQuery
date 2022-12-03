# 天气查询快捷指令

> **冬天来了,提前查询室外天气,以防感冒~**

## 接口来源

> 天气  | 精度维度 查询API -> [msn天气](https://www.msn.cn/zh-cn/weather/forecast/in-%E5%8C%97%E4%BA%AC%E5%B8%82?loc=eyJsIjoi5YyX5Lqs5biCIiwiYyI6IuS4reWNjuS6uuawkeWFseWSjOWbvSIsImkiOiJjbiIsInQiOjEwMiwiZyI6InpoLWNuIiwieCI6IjExNi40MDc0MTciLCJ5IjoiMzkuOTA0MTcyIn0%3D&weadegreetype=C)

## 安装地址

iCloud分享链接: https://www.icloud.com/shortcuts/7e356196396c46c7a3b3be6af4eaffa6

## 实现思路

查询某地的天气 -> API获取 -> 经度和纬度

天气查询接口 -> 拼接经度和维度参数

> 两种查询天气方式:
>
> > 获取当前天气:
> >
> > 将天气查询API 参数num替换为10 ->  请求API -> 通过词典获取对应的天气信息
> >
> > > **获取天气预报信息**
> > >
> > > 由于不同地区天气预报信息长度不一样，所以需要判断
> > >
> > > 但是长度2是固定的,但是3是不固定的。
> > >
> > > 判断当长度 > 2时 获取 数组3当中的元素值.
>
> > 获取未来天气:
> >
> > 请求输入要查询的天气天数 -> 将天气查询API 参数num替换为输入要查询的天气天数 ->  请求API -> 通过词典获取对应的天气信息

