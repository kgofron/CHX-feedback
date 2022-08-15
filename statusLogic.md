# Global feedback

```
For the x-direction (y-should be self-explaining)

feedback_on_pv = SR:FOFB{}FOFBOn

x_actions_done_pv = SR:APHLA:SOFB{BUMP:C11-CHX}X-CmdDone
x_offset_RB_pv = SR:APHLA:SOFB{BUMP:C11-CHX}offset:X-I
x_offset_SP_pv = SR:APHLA:SOFB{BUMP:C11-CHX}offset:X-SP
x_angle_RB_pv = SR:APHLA:SOFB{BUMP:C11-CHX}angle:X-I
x_angle_SP_pv = SR:APHLA:SOFB{BUMP:C11-CHX}angle:X-SP


Logic for 'Bump X':

feedback_on_pv && x_actions_done_pv && (abs(x_offset_SP_pv-x_offset_RB_pv) < .003) && (abs(x_angle_SP_pv-x_angle_RB_pv) < .0015)
```