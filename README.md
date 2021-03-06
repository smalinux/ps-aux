# ps-aux
Simple easy-to-use Linux kernel module takes PID from users as input, then expose some info into dmesg.

## Download
```
git clone https://github.com/smalinux/ps-aux
cd ps-aux
```

## Build and installation
```
make all
sudo make i
```
## How to use
```
echo PID > /dev/sma_chardev
make p
```

That's it!

Make utilities:
* $make i == insmod
* $make p == print dmesg
* $make c == Clear dmesg
* $make r == rmmod
* $make info == modinfo
* $make clear == clear!

### My TODO list
* Read about virtual memory from mm_struct.
* list children of a proc properly.
* Print recurve PID info.
* Not use dmesg any more, Make a virtual fs.

### My references
* linux cross reference
* man proc
* My [silly](https://stackoverflow.com/q/61211757/5688267) related [questions](https://stackoverflow.com/q/61295277/5688267) on StackOverflow! :D

> Special thanks to my great mentor [M.Samman](https://github.com/sammantic). :heart:  
If you have any question related or you want to just say hi, feel free. telegram: [@smalinux](https://web.telegram.org/@smalinux)
