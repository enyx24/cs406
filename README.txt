--- DANH SÁCH THÀNH VIÊN ---
Nguyễn Thái Học - 22520488
Nguyễn Duy Khang - 22520619
Nguyễn Quốc Hưng - 22520516
Nguyễn Trọng Nhân - 22521005

--- LINK DATASET ---
https://drive.google.com/file/d/1WNy9IapqRqmSOTDVBzBY9YpHS_DhnjKF/view?usp=sharing

--- LINK SOURCE CODE---
https://github.com/enyx24/cs406

--- HƯỚNG DẪN CÀI ĐẶT MÔI TRƯỜNG ẢO ---

*** YÊU CẦU ***
Anaconda Prompt (miniconda3)
nvcc
nvidia driver

*** CÀI ĐẶT ***
# Chạy trong miniconda3 promt
git clone https://github.com/enyx24/cs406
cd cs406
conda env create --file environment.yml

--- TRAINING ---

*** YÊU CẦU ***
Giải nén thư mục train vào thư mục ssd / adssd

*** TRAIN ***
	+ Mở miniconda3 tại thư mục ssd hoặc adssd
	+ conda activate pytorch_env
	+ python -m tools.train
--- EVALUATION ---

*** YÊU CẦU ***
Giải nén 2 thư mục train vào thư mục ssd / adssd

*** EVALUATION ***
	+ Mở miniconda3 tại thư mục ssd hoặc adssd
	+ conda activate pytorch_env
	+ python -m tools.infer --evaluate True --infer_samples False

*** DEMO ***
	+ Mở miniconda3 tại thư mục làm việc chính (cs406)
	+ conda activate pytorch_env
	+ streamlit run demo.py

