# DP����
```csharp
// From M1s.cs
// ��Ŀ��ʼ��ȡλ�������ң���һ��list����TargetOrderIndex����˭������
dp.TargetResolvePattern = PositionResolvePatternEnum.PlayerNearestOrder;
dp.TargetOrderIndex = 2;
// Delay��ʱ�����Ծ���SendDraw���û���
dp.Delay = 6000 + Interval;
dp.DestoryAt = 3000 - Interval;
```

```csharp
// From M1s.cs
// �����������
[ScriptMethod(name: "P3�������߼���", eventType: EventTypeEnum.Tether, eventCondition: ["Id:0066"])]
// ͬʱ����������о�
[ScriptMethod(name: "�ذ��޸���ȫ��", eventType: EventTypeEnum.EnvControl, eventCondition: ["Id:00080004", "Index:regex:^(0000000[1247])$"])]
// ���������п����
if (@event["Index"] == "00000001")
```