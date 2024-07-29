# SEVAR: A Stereo Event Camera Dataset for Virtual and Augmented Reality

## ABSTRACT:
Event cameras, characterized by their low latency,large dynamic range, and extremely high temporal resolution, have recently received increasing attention.These features make them particularly well-suited for virtual/augmented reality (VR/AR) applications. To facilitate the development of three-dimensional (3D)perception and navigation algorithms in VR/AR applications using event cameras, we introduce the Stereo Event camera dataset for Virtual and Augmented Reality (SEVAR), which comprises a wide variety of head-mounted indoor sequences, including scenarios with rapid motion and a large dynamic range. We present the first comprehensive set of VR/AR datasets captured with an event-based stereo camera, a regular stereo camera at 30 Hz, and an inertial measurement unit at 1000 Hz. The camera placement, field of view (FoV), and resolution match those of the head-mounted device, such as Meta Quest Pro. All sensors are time-synchronized in the hardware. Ground truth poses captured by a motion capture system are also available for trajectory evaluation. The sequences include several common scenarios, and cover the specific challenges targeted by event cameras.

## MAIN CONTRIBUTIONS:
*  We present the first event-based dataset explicitly designed for VR and AR scenarios in terms of camera placement, FoV angle, and resolution.
*  We provide a variety of motion modes, indoor settings, and lighting conditions, offering sequences that span from easy to extremely challenging scenarios.Furthermore, we have incorporated other challenging situations commonly encountered in practical applications of head-mounted devices, such as picking up items and rapid head movements.
* The datasets are captured by a precisely hardware synchronized sensor suite that includes a stereo event camera, a stereo regular camera, and an inertial measurement unit (IMU), simultaneously recording a six-degree-of-freedom (6-DoF) ground truth pose for each sequence.

## SENSOR SETUP
IMU (middle), stereo regular cameras (bottom), and event cameras (top) are rigidly mounted on a 3D-printed holder
![image](https://github.com/sevar-dataset/sevar/blob/main/Fig1.png,width="800px")
* **RGB Camera** OV7251; 640×480; f/0.825 mm; FoV: 165° D-FOV; global shutter; 30 Hz.
* **Event Camera** DAVIS346; 346×260; f/2.8 mm; FoV: 150° D-FOV; up to 120 dB.
* **IMU**  ICM42688P; 3-axis accelerometer; 3-axis gyroscope; 1000 Hz.
* **Motion-capture System** Vicon Vero 2.2; localization accuracy 1mm; 300 Hz.

## DATASET SEQUENCES
Sequence Name|Total Size|Duration|Rosbag|GT
--|:--|:--:|--:|--:
AR-normal|2.28g|92s|[Rosbag](https://pan.baidu.com/s/1zvpk3hRYwEopyPsoF6WshA )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EeWoHTQA1QtCk0tByN716boBsaj-6KRwnviLcxNZXlqWMA?e=7Af0jd)
AR-hdr|3.03g|98s|[Rosbag](https://pan.baidu.com/s/10iftQF62biYDjtBSby_HXg )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/ESrI-6U_KU5Ns54_CNN4jGYBgd_o71BTwBbdNDwN4F9NTg?e=EYrIVi)
VR-normal|2.88g|80s|[Rosbag](https://pan.baidu.com/s/1HEZrGog6FkdV3ppShSTsFg )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EVhB8s1AlqdFrMVp4o4g_DoB3GqabFZ7rOmprJ3qDWNoXg?e=PcpEOj)
VR-hdr|2.45g|86s|[Rosbag](https://pan.baidu.com/s/1jiG0SHdFdQ15S0XpextSfA )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EXC0AhGF76VCv6U02hDiFQsBTA0r_LKgpcqHyK5p-zSzvA?e=R3YwF1)
Board-slow|0.61g|21s|[Rosbag](https://pan.baidu.com/s/1z4NnnJe7WXNBy41_iEcfYQ )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EcfDi3SwX7RFtJU1RAyO2KMBGwqTe6ntZw3jckGryfDMkg?e=JLeWH0)
Board-normal|1.30g|25s|[Rosbag](https://pan.baidu.com/s/134dtmmuVqq83FshuZg4TyQ )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EciLEcak0KZJmHXXBwNRMCgB4PNLzpjUmuPwHh5tKTQk-Q?e=loeyWv)
Board-fast|2.79g|23s|[Rosbag](https://pan.baidu.com/s/1uZSBUJs8fe6wgtArOKO-pw )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/ESHQVmqu0b1Jun-db3TxzRgBQMDycFducz8UmSlNcPK7xA?e=j2azvV)
Board-hdr|0.97g|25s|[Rosbag](https://pan.baidu.com/s/1EZ6wwSO5CICVXkwd94CseQ )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EUm7wPhhMYpJndDCZdGwbCgBAstKpKeKINYh8EljoWNrsw?e=hJfnTF)
Desk-normal|1.54g|57s|[Rosbag](https://pan.baidu.com/s/1In7j60PcgHsr87-wwhAMwg )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/ESPLFC29HchEquE3akbo_60Brd5q6lID0U9gc8dtVallFg?e=AvBn8s)
Desk-fast|2.69g|53s|[Rosbag](https://pan.baidu.com/s/1d9eSR91Fbub5GARINvUGzg )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/ESZKLTyAJopNtRwpci9_WCcBbXhZ3UJwFZzOr_a3xb6Ozg?e=Fn8aoM)
Desk-hdr|2.37g|50s|[Rosbag](https://pan.baidu.com/s/1pNlWreWqqARHWRbuhNPuQQ )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EQ3mIkFWfkZJqp2bLpsgQB4BKLUoZ0lsPLSdqQ4Kyr_hzA?e=yZysT9)
Walk-slow|1.16g|51s|[Rosbag](https://pan.baidu.com/s/1Z6873JGBz6OqFlnetDDuLQ )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/Ee-qZdqIREBDozHGLSsUI8wB1zCN8sqy0P-7j73Qp_S-Bw?e=PKgh17)
Walk-normal|1.30g|58s|[Rosbag](https://pan.baidu.com/s/1DfLbd3X6tfjdce1wxp9V5w )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EaQu1pG_JN5Og9SQpe_dpF0Bgv7fO7PitPotX7k-C-SBfA?e=grLSwq)
Sofa-normal|0.75g|30s|[Rosbag](https://pan.baidu.com/s/1Gfeot6yZqqaCaVT_UBPMQA )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EY3rW8noaFFOldg6yakm02UBmj9xHw45zF1x2zQCPA9xIQ?e=VZFOYI)
Sofa-fast|2.09g|35s|[Rosbag](https://pan.baidu.com/s/17KyEHO5KvXPORZ2BV0iFHw )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EXOuVL0YV_NMt3ZtfCW949ABErpuFnNBixKqPd8amOvr0Q?e=jQEiT8)
Sofa-hdr|1.01g|33s|[Rosbag](https://pan.baidu.com/s/1Amgejb5WlFSIyA4hxj3Jzg )|[GT](https://1drv.ms/t/c/48c1f55133f3a070/EYG3hTMpmLZMk2r94t2AnW4B6i1YufTE3us65yDMe8YSSw?e=wniUeT)

### Calibration
  For camera intrinsics,visit [Ocamcalib](http://sites.google.com/site/scarabotix/ocamcalib-toolbox)  
  for omnidirectional model.visit [Vins-Fusion](https://github.com/HKUST-Aerial-Robotics/VINS-Fusion)  
  for pinhole and MEI model.use [Opencv](https://opencv.org/) for Kannala Brandt model  
  For IMU intrinsics,visit [Imu_utils](https://github.com/gaowenliang/imu_utils)  
  For extrinsics between cameras and IMU,visit [Kalibr](https://github.com/ethz-asl/kalibr)  
