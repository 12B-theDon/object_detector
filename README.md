# object_detection
object detection for detecting wall and dynamic&amp;static obstacles

## TODO
### 의존성 설치  
cd object_detector  
pip install -r requirements.txt  

### cordinate.py import  
object_detector/src/tracker.py 내의   
sys.path.append('#해당 directory#/cordinate/src') -> directory 수정  

### cordinate config path 수정
cordinate/config 내의   
map&global path path 수정  

### 패키지 빌드  
cd ..  
colcon build   

### frenet_converter & globalpath_loader 실행  
cd cordinate  
source install/setup.bash  
ros2 run cordinate cordinate_converter  

### object detector & tracker 실행  
cd object_detector  
source install/setup.bash  
ros2 launch object_detector object_detect_launch.py  

