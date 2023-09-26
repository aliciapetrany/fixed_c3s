# fixed_c3s
This is a modified __init__.py file for C3S so that it works on modern linux machines  

Once you have gotten to the runc3s.py step in the homework,  
1. Download __init__.py from this repository   
2. Open a new terminal, and run the following code one line at a time:  
```
conda activate YONG-C3S
cd C3S
cp ~/Downloads/__init__.py src/
python setup.py install --user 
```
3. Open your web browser, and download the SRA files MANUALLY from these links. It WILL NOT WORK if you use the wget links.  
```
https://drive.google.com/file/d/1tHhPFmEZ0SUKHh4MoTK5vP3Xl5Mjp8G9/view?usp=sharing
https://drive.google.com/file/d/1lN8ahayDZUzuO8auyzonIzoyacx7RdMF/view?usp=sharing

```
4. Move those SRA files from your downloads folder into your C3S folder
5. Run the pipline with:
```
runC3S.py -x hg19_basic -1 SRR5583324_1.fastq.gz -2 SRR5583324_2.fastq.gz --prefix HS3 --bait chr11:5305934
```
