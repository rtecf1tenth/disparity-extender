# Improved Disparity Extender Autonomous Racing Algorithm
Built on top of https://github.com/cs496-f1tenth/william-full-stack

### To launch the car’s controllers run
```python
ros2 launch william_full_stack bringup.py
```
- this script enables the car to be driven manually
- toggles the killswitch (LB). This button needs to be pressed for disparity messages to be sent through to the VESC

### To launch the disparity listener run
```python
ros2 launch willam_full_stack DE.launch.py
```
### To start the disparity algorithm run

```python
python3 disparity.py
```
### Notes:
- Needs tuning depending on the environment. Generally the standalone script works with wider tracks but needs tuning as the track gets more narrow.
- Some values we had to play with were `KP, KD, SAFETY_PERCENTAGE,` and `VIEW_RANGE` .
