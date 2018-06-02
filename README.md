# robit Package
This ElecFreaks robit package was developed by [ElecFreaks](https://www.elecfreaks.com/) with minor assistance from [Tinkercademy](https://tinkercademy.com/).


## Code Example
```JavaScript
robit.init_line_follow(robit.Jpin.J1)
basic.forever(() => {
    if (robit.left_line_follow() == 1 && robit.right_line_follow() == 0) {
        robit.MotorRunDual(
        robit.Motors.M1,
        25,
        robit.Motors.M2,
        0
        )
    } else if (robit.left_line_follow() == 0 && robit.right_line_follow() == 1) {
        robit.MotorRunDual(
        robit.Motors.M1,
        0,
        robit.Motors.M2,
        25
        )
    } else {
        robit.MotorRunDual(
        robit.Motors.M1,
        10,
        robit.Motors.M2,
        10
        )
    }
})

```

## License
MIT

## Supported targets
for PXT/microbit (The metadata above is needed for package search.)

