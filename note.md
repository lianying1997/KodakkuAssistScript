# DP函数
```csharp
// From M1s.cs
// 将目标始终取位最近的玩家，做一个list，由TargetOrderIndex决定谁离得最近
dp.TargetResolvePattern = PositionResolvePatternEnum.PlayerNearestOrder;
dp.TargetOrderIndex = 2;
// Delay延时，可以决定SendDraw后多久画画
dp.Delay = 6000 + Interval;
dp.DestoryAt = 3000 - Interval;
```

```csharp
// From M1s.cs
// 分身连线相关
[ScriptMethod(name: "P3分身连线技能", eventType: EventTypeEnum.Tether, eventCondition: ["Id:0066"])]
// 同时满足两项的判决
[ScriptMethod(name: "地板修复安全区", eventType: EventTypeEnum.EnvControl, eventCondition: ["Id:00080004", "Index:regex:^(0000000[1247])$"])]
// 后续代码中可添加
if (@event["Index"] == "00000001")
```