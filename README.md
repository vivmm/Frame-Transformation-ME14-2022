# 2D frame transformation

From image coordinate to 2D (BEV) world coordinate

![image](https://github.com/vivmm/ME14_2022/assets/103901978/4f0a12ee-c2fa-4090-a93e-c40092c61bef)

## Recommended System Setup
- Windows 10
- Python 3.10.5
- OpenCV 4.6.0

## How to use
**Find_dst_src_for_Homogarphy.ipynb >> Average_point.ipynb >> Frame_Transformation_2D.ipynb >> Velocity_filtering.ipynb >> plot_BEV.ipynb**

1. run Find_dst_src_for_Homogarphy.ipynb จะได้ตำแหน่ง src และ dst ออกมาเป็นไฟล์ src.out และ dst.out

![image](https://github.com/vivmm/ME14_2022/assets/103901978/4d682772-2e93-4dd9-a37c-c3cf4bec75ac) ![image](https://github.com/vivmm/ME14_2022/assets/103901978/c348d695-7c5b-435b-b5cd-65d0b6fc2a3c)

![image](https://github.com/vivmm/ME14_2022/assets/103901978/3d1befe4-801a-4efe-b292-5b6941ccfa6f) ![image](https://github.com/vivmm/ME14_2022/assets/103901978/ed322bfb-2fc9-42b5-95ad-bf932037a6f5)

2. หาตำแหน่งเฉลี่ยจากการคลิกหลาย ๆ ครั้งด้วย Average_point.ipynb
3. input src.out, dst.out และ trajectory ใน image coordinate ให้กับ Frame_Transformation_2D.ipynb จะได้ Homography และ trajectory ใน world coordinate

format ของ trajectory ใน image coordinate

![image](https://github.com/vivmm/ME14_2022/assets/103901978/cef8b390-db93-408c-8add-2285870c04c6)

format ของ trajectory ใน world coordinate

![image](https://github.com/vivmm/ME14_2022/assets/103901978/644e51ef-9a69-4d5e-a738-5c5466df0a28)

4. filter track ที่มีปัญหาด้วย Velocity_filtering.ipynb จะได้ track id ที่มีปัญหา
5. vizualization ด้วย plot_BEV.ipynb

![image](https://github.com/vivmm/ME14_2022/assets/103901978/13230842-791e-4fb5-9353-c5e50cc6d136)


