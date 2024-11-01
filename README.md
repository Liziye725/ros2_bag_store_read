```
mkdir ros2bag
cd ros2bag/
```
```
ros2 bag record /fix -o fix_test_20241101
```
```
ros2 bag info fix_test_20241101
```

Play it: open in two terminal, one run `ros2 bag play [file_name]`, another run `ros2 topic echo /[topic_name]`.

cd to the path where .bag stored:
```
cd /home/ziye/Documents/maps/ros2bag
```
```
source ~/gnss_ws/install/setup.bash
```
```
ros2 bag play fix_test_20241101
```
```
ros2 topic echo /fix
```
