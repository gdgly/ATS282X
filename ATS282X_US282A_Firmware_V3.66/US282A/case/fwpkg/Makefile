# ��makefile�����Զ���ɹ������ã�������룬�̼����ɵȹ��ܣ������ʵ������޸ĸ�makefile���Է���
# ��������Ĺ̼�
# makefile���������shell�ļ�
#       config.sh���ڹ������ã��ɸ������õİ��ͺ͹����Ƿ�֧�֣����޸Ĳ����ļ�����ɹ�����Ĵ򿪺͹ر�
#       make.sh ����Դ������룬��shell�ű������case/cfgĿ¼�µ�makefile���г������
#       build.sh ���ڹ̼����ɣ��ɸ������õİ��ͺ͹����Ƿ�֧�֣�������Ӧ��Ŀ��̼����ýű�������fw�ļ�������������������
#                hex��fwu�ļ������������ܣ�atf�ļ�����ATT�����Զ������ԣ��Լ�OTA�ļ�����apk����
# ������ù����У���һ��shell�ű�������������������̻�ֹͣ������������shell�ű������������Ӧ��log�ļ�����ͨ������log�ļ���������ԭ��

# ���������һ��֧��TWS���ܵ�ATS2823�Ĺ̼�����������������make clean;make DVB_ATS2823_TWS,���Կ���DVB_ATS2823_TWS��һ��αĿ�꣬��Ŀ������
# config.sh,��TWS���ܴ򿪡����ŵ���make.sh��build.sh��ɹ̼�������

# ���֮ǰԴ�����Ѿ��������ֻ���޸���ĳ���ļ������ٴ����ɹ̼���������make DVB_ATS2823_TWS,��ɳ���ı���

# ���Դ�ļ���û���޸ģ�����ֻ���ٴ����ɹ̼���������make build_DVB_ATS2823_TWS��make build��ɹ̼�������

# ��ʼʱ��
TIME_BEGIN := $(shell (date +%s))

.PHONY : all clean clean_target test

DVB_ATS2825:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
EVB:
	./config.sh ./config_txt/US282A_BTBOX_EVB.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_EVB.ini 2>&1 | tee ./build.log		
	@echo EVB: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2823:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2823.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2823: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds	

DVB_ATS2823T:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2823T.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823T.ini 2>&1 | tee ./build.log
	@echo DVB_ATS2823T: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2823B:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2823B.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823B.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2823B: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
EVB_OTA:
	./config.sh ./config_txt/US282A_BTBOX_EVB_OTA.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_EVB_OTA.ini 2>&1 | tee ./build.log	
	@echo EVB_OTA: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2825_OTA:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_OTA.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_OTA.ini 2>&1 | tee ./build.log	

	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_OTA_1M.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_OTA_1M.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825_OTA: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
EVB_TWS:
	./config.sh ./config_txt/US282A_BTBOX_EVB_TWS.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_EVB_TWS.ini 2>&1 | tee ./build.log
	@echo EVB_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2825_TWS:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
		
DVB_ATS2825_TWS_ESD:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_ESD.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_ESD.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825_TWS_ESD: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2825_TWS_48K:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_48K.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_48K.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825_TWS_48K: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds

DVB_ATS2825_TWS_BQB:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_BQB.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_BQB.ini 2>&1 | tee ./build.log
	@echo DVB_ATS2825_TWS_BQB: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds	
			
DVB_ATS2823_TWS:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_TWS.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_TWS.ini 2>&1 | tee ./build.log
	@echo DVB_ATS2823_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2823W:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_W.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_W.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2823W: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds

DVB_ATS2825W:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_W.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_W.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825W: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds

EVB_W:
	./config.sh ./config_txt/US282A_BTBOX_EVB_W.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_EVB_W.ini 2>&1 | tee ./build.log	
	@echo EVB_W: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds	

DVB_ATS2823W_TWS:	
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_TWS_W.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_TWS_W.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2823W_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds

DVB_ATS2825W_TWS:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_W.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_W.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825W_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
DVB_ATS2825CW:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_CW.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_CW.ini 2>&1 | tee ./build.log
	@echo DVB_ATS2825CW: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds	

DVB_ATS2825CW_TWS:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825CW_TWS.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825CW_TWS.ini 2>&1 | tee ./build.log
	@echo DVB_ATS2825CW_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds	
		
DVB_ATS2825C_TWS:
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825C_TWS.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825C_TWS.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825C_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds

DVB_ATS2825_TWS_LOW_DELAY: 
	./config.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_LOW_DELAY.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_LOW_DELAY.ini 2>&1 | tee ./build.log	
	@echo DVB_ATS2825_TWS_LOW_DELAY: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds

EVB_W_TWS:
	./config.sh ./config_txt/US282A_BTBOX_EVB_TWS_W.ini 2>&1 | tee ./config.log
	./make.sh 2 2>&1 | tee ./make.log
	./build.sh ./config_txt/US282A_BTBOX_EVB_TWS_W.ini 2>&1 | tee ./build.log
	@echo EVB_W_TWS: all, $$[$$(date +%s)-$(TIME_BEGIN)] seconds
	
build_EVB:
	./build.sh ./config_txt/US282A_BTBOX_EVB.ini 2>&1 | tee ./build.log    	
build_EVB_W:
	./build.sh ./config_txt/US282A_BTBOX_EVB_W.ini 2>&1 | tee ./build.log  
	
build_DVB_ATS2825:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825.ini 2>&1 | tee ./build.log	
	
build_DVB_ATS2825W:	
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_W.ini 2>&1 | tee ./build.log		

build_DVB_ATS2823:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823.ini 2>&1 | tee ./build.log
	
build_DVB_ATS2823W:	
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_W.ini 2>&1 | tee ./build.log			

build_DVB_ATS2823T:	
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823T.ini 2>&1 | tee ./build.log	
	
build_DVB_ATS2823B:	
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823B.ini 2>&1 | tee ./build.log
		
build_EVB_OTA:
	./build.sh ./config_txt/US282A_BTBOX_EVB_OTA.ini 2>&1 | tee ./build.log	

build_DVB_ATS2825_OTA:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_OTA.ini 2>&1 | tee ./build.log
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_OTA_1M.ini 2>&1 | tee ./build.log
build_EVB_TWS:
	./build.sh ./config_txt/US282A_BTBOX_EVB_TWS.ini 2>&1 | tee ./build.log

build_DVB_ATS2825_TWS:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS.ini 2>&1 | tee ./build.log
	
build_DVB_ATS2825_TWS_48K:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_48K.ini 2>&1 | tee ./build.log

build_DVB_ATS2825_TWS_BQB:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_BQB.ini 2>&1 | tee ./build.log	
	
build_DVB_ATS2825CW:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_CW.ini 2>&1 | tee ./build.log	

build_DVB_ATS2825CW_TWS:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825CW_TWS.ini 2>&1 | tee ./build.log	
	
build_DVB_ATS2825C_TWS:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825C_TWS.ini 2>&1 | tee ./build.log		

build_DVB_ATS2825_TWS_LOW_DELAY:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_LOW_DELAY.ini 2>&1 | tee ./build.log	

build_DVB_ATS2823_TWS:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2823_TWS.ini 2>&1 | tee ./build.log	
	
build_DVB_W_TWS:
	./build.sh ./config_txt/US282A_BTBOX_DVB_ATS2825_TWS_W.ini 2>&1 | tee ./build.log
	
build_EVB_W_TWS:
	./build.sh ./config_txt/US282A_BTBOX_EVB_TWS_W.ini 2>&1 | tee ./build.log
all:
	make clean;make EVB_TWS
	make clean;make DVB_ATS2825
	make clean;make DVB_ATS2825W	
	make clean;make DVB_ATS2825_TWS
	make clean;make DVB_ATS2825W_TWS
	make clean;make DVB_ATS2823_TWS
	make clean;make DVB_ATS2823W_TWS	
	make clean;make DVB_ATS2825_OTA		
	make clean;make DVB_ATS2825_TWS_ESD	
	make clean;make DVB_ATS2823T
	make clean;make DVB_ATS2825_TWS_48K

test:
	#make clean;make EVB
	#make clean;make DVB_ATS2825
	#make clean;make DVB_ATS2823
	#make clean;make EVB_OTA
	#make clean;make EVB_TWS
	#make clean;make DVB_ATS2825W
	#make clean;make DVB_ATS2823W		
	#make clean;make DVB_ATS2825_TWS
	make clean;make DVB_ATS2823_TWS
	#make clean;make DVB_ATS2823W_TWS	
	#make clean;make DVB_ATS2825_OTA
	#make clean;make DVB_ATS2825CW_TWS
	make clean;make DVB_ATS2825_TWS_LOW_DELAY
	make clean;make DVB_ATS2825W_TWS
	make clean;make DVB_ATS2825_TWS	
build:
	./build.sh  2>&1 | tee ./build.log  
	  
clean:
	./make.sh 0 2>&1 | tee ./make.log

clean_target:
	./make.sh 1 2>&1 | tee ./make.log