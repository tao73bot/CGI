# CGI Labtask

### Task1- Bresensam Line Drawing Algorithm

This algorithm is used for scan converting a line. It was developed by Bresensam. It is an efficient method because it involves only integer addition, subtractions, and multiplication operations. These operations can be performed very rapidly so lines can be generated quickly.

Assume a pixel P1'(x1',y1'),then select subsequent pixels as we work our may to the night, one pixel position at a time in the horizontal direction toward P2'(x2',y2').

The line is best approximated by those pixels that fall the least distance from the path between P1',P2'.

![App Screenshot](https://static.javatpoint.com/tutorial/computer-graphics/images/computer-graphics-bresenhams-line-algorithm.jpg)


### Adjustments for m > 1
Bresenham algorithm only work for `0 < slope < 1`. As we have to make `m < 1` so I swaped the `(x1,y1) with (y1,x1)` and `(x2,y2) with (y2,x2)`. 

### Result
- case-1: `(1,1),(8,4)`
    - Result
    `(1, 1),
    (2, 1),
    (3, 2),
    (4, 2),
    (5, 3),
    (6, 3),
    (7, 4),
    (8, 4)
    `

- case-2 `(1,1), (4,8)`
    - Result
    `(1, 1)
    (1, 2)
    (2, 3)
    (2, 4)
    (3, 5)
    (3, 6)
    (4, 7)
    (4, 8)
    `