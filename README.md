# Murphi-dt4
Murphi-dt4 is a variant of paraVerifier server. Unlike the paraVerifier server, Murphi-dt4 uses the decision tree mechanism to filter the candidate invariants sent by the client of paraVerifier. Compared with the normal paraVerifier server, Murphi-dt4 can use less memory to judge the correctness of candidate invariants, thus reducing the memory requirements of protocol validation.


# Background
paraVerifier : https://github.com/lyj238Gmail/newParaVerifier#paraverifier

# Requirements
Same as the requirements of the paraVerifier server part.

# Installation
Decompress two compressed packages. (server-dt4.tar.gz ; murphi_r_2.tar.gz)

# Run an example
1.Open the extracted folder of server-dt4.tar.gz.  
2.Modify the file settings.py. Set SMV_PATH, MU_PATH, MU_INCLUDE, GXX_PATH according to system parameters. SMV_PATH is the path of NuSMV. MU_PATH is the path of Mu file after extracting murphi_r_2.tar.gz file. MU_INCLUDE is the path of the include file after extracting murphi_r_2.tar.gz file. GXX_PATH is the path of g++.  
3.Run the server. Run the server with the command "python server.py".  

# Experiments
We have applied Murphi-dt4 to a number of benchmarks:

protocol  | time/s  | memory/MB  
---- | ----- | ------    
Mutual Exclusion  | 8.39 | 25  
MOESI  | 4.67 | 25    
MESI  | 4.67 | 25    
German  | 64.89 | 42    
Flash_nodata  | 1185.09 | 511    
Flash  | 7152.68 | 3200    




  

# Murphi-dt4 (CHINESE)
Murphi-dt4是协议验证软件paraVerifier服务器部分的变种。与paraVerifie服务器不同的是，Murphi-dt4使用决策树机制筛选paraVerifie客户端发来的候选不变式。相较于原版paraVerifier服务器，Murphi-dt4能够使用更少的内存判断候选不变式的正确性，从而减少协议验证对内存的要求。

# Background
paraVerifier详见https://github.com/lyj238Gmail/newParaVerifier#paraverifier

# Requirements
与paraVerifie服务器部分要求相同。

# Installation
解压两个压缩包(server-dt4.tar.gz ; murphi_r_2.tar.gz)

# Run an example
1. 打开server-dt4.tar.gz解压后的文件夹。  
2. 修改settings.py文件，根据系统参数设置SMV_PATH，MU_PATH，MU_INCLUDE，GXX_PATH，其中SMV_PATH为NuSMV的路径，MU_PATH为murphi_r_2.tar.gz文件解压后mu文件的路径，MU_INCLUDE为murphi_r_2.tar.gz文件解压后include文件的路径，GXX_PATH为g++的路径。  
3. 运行服务器。使用命令python server.py运行客户端。
# Experiments
Murphi-dt4已应用于以下实验

protocol  | time/s  | memory/MB  
---- | ----- | ------    
Mutual Exclusion  | 8.39 | 25  
MOESI  | 4.67 | 25    
MESI  | 4.67 | 25    
German  | 64.89 | 42    
Flash_nodata  | 1185.09 | 511    
Flash  | 7152.68 | 3200    

