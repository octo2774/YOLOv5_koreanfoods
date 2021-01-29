# YOLOv5_koreanfoods

#1
크롤링 or chrome scripper 로 사용할 이미지 수집 (여기서는 만두, 치즈, 새우튀김)

#2
수집한 파일을 https://cvat.org/ 에서 전처리
(Create new Task → jobs 에서 job#~~~ 클릭 → 사각형 툴로 rectangle 일일히 다 지정해주고 → task로 돌아와서 action: export as a dataset (PASCAL VOC1.1))

#3 export 한 파일을 roboflow 에 업로드
(Creatae dataset, 모든 파일은 train 100%로, object decation(bounidng) 으로 해야 xml파일 업로드 가능, xml 파일과 image 파일을 동시에 업로드해야함)

#4 업로드 한 파일을 YOLOv5 tutorial 을 참고해서 cobal 에서 프로그램 구성

