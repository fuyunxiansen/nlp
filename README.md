*重要：*
基础环境：GCC-11,PYTHON 3.10

WINDOWS未测试
最好用WSL

cd PolyUGPT

pip install -r requirements.txt

CMAKE_ARGS="-DLLAMA_CUBLAS=on" FORCE_CMAKE=1 pip install llama-cpp-python==0.1.83 --no-cache-dir

处理文本：
python PolyUGPT/ingest.py
（已处理 可省略）

CMD运行：第一次运行会下载模型LLAMA-7B-CHAT
python PolyUGPT/run_PolyUGPT.py

WEBUI运行：
python PolyUGPT/run_PolyUGPT_API.py
