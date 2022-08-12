# Feedback logic

## x-Bump

```
PV:
SR:APHLA:LBAgent{BUMP:C11-CHX}X-FdbkEnabled
--------
0: SR:APHLA:LBAgent{BUMP:C11-CHX}X-FdbkEnabled.RVAL
1: SR:APHLA:LBAgent{}Enable-Cmd.RVAL
2: SR:APHLA:LBAgent{BUMP:C11-CHX}X-AgentActionComment
--------
green: (pv0 == 1) && (pv1 == 1) && (pv2 == 4)
red: ! ((pv0 == 1) && (pv1 == 1) && (pv2 == 4))
```

## y-Bump

```
PV:
SR:APHLA:LBAgent{BUMP:C11-CHX}Y-FdbkEnabled
--------
0:  SR:APHLA:LBAgent{BUMP:C11-CHX}Y-FdbkEnabled.RVAL
1:  SR:APHLA:LBAgent{}Enable-Cmd.RVAL
2:  SR:APHLA:LBAgent{BUMP:C11-CHX}Y-AgentActionComment
--------
greee: (pv0==1)&&(pv1==1)&&(pv2==4)
red:   !((pv0==1)&&(pv1==1)&&(pv2==4))
```