
## **___Input Key___**


###### Visual Studio code 설치후 사용가능.

```
import curses

def main(stdscr):
    while True:
        key = stdscr.getch()

        if key == curses.KEY_UP:
            print("You pressed the up arrow.")
        elif key == curses.KEY_DOWN:
            print("You pressed the down arrow.")
        elif key == curses.KEY_LEFT:
            print("You pressed the left arrow.")
        elif key == curses.KEY_RIGHT:
            print("You pressed the right arrow.")
        elif key == ord('q'):
            print("You pressed 'q'. Exiting...")
            break

curses.wrapper(main)
```

---

<!--목차 & 다음으로 페이지 이동-->
[목차](https://github.com/Devcurve/Python/blob/main/README.md)<br>
[이전 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/class.md)<br>
<!--[다음 페이지](https://github.com/Devcurve/Python/blob/main/Chapter_2/InputKey.md)-->
