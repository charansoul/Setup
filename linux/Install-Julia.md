# How to setup Julia on linux distros or servers:

## Introduction to Julia:
Julia represents a cutting-edge and versatile programming language renowned for its impressive equilibrium between expressive power at a high level and remarkable performance.

Engineered to cater to the demands of both general-purpose programming and high-performance scientific computing, Julia has gained significant traction in diverse fields such as data science, numerical analysis, machine learning, and computational research.

One of the standout attributes of Julia lies in its capacity to amalgamate the ease of use and readability found in conventional high-level languages like Python with the raw computational muscle of languages such as C or Fortran. This feat is achieved through a just-in-time (JIT) compiler that generates optimized machine code in real-time, allowing Julia programs to rival the speed of languages compiled natively.

Moreover, Julia's type system and architecture for multiple dispatch exhibit elegance and efficiency in code organization. This means that functions can be specialized for various argument types, empowering developers to create code that is both versatile and highly efficient.

The language's wide-ranging collection of packages and libraries form a rich ecosystem that provides a wealth of tools for data manipulation, visualization, mathematical computation, and more.

Due to its exceptional performance capabilities, Julia has found particular favor among scientists, engineers, and researchers who require swift prototyping and execution of intricate numerical algorithms. Its seamless integration with existing C and Fortran codebases allows for easy utilization of legacy code while harnessing the modern features of Julia.

In summary, Julia's unique combination of expressive power at a high level, dynamic nature, and exceptional performance establishes it as a formidable choice for a broad spectrum of programming tasks, particularly those involving numerical analysis, data manipulation, and scientific computing.

Find more about Julia [here](https://docs.julialang.org/). 

### Installation:
1. **Open a Terminal:** Launch your terminal application.
2. **Navigate to Downloads Folder:** Change your current working directory to the Downloads folder using the `cd` command. This is done by typing:   
   ```bash
   cd ~/Downloads
3. **Download Julia Linux Binaries:** Use the wget command to download the latest compressed Julia Linux Binaries from the official Julia website. The command is:
    ```bash
    sudo wget --no-check-certificate https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.2-linux-x86_64.tar.gz
* Alternate setup if the above link is not working:
    ```bash
    wget https://nftstorage.link/ipfs/bafybeibbpcxtgaxla5dl3tuzfe3qlozaga5zqpybe5dfuhehtqdpsk6t54
* IPFS CID: bafybeibbpcxtgaxla5dl3tuzfe3qlozaga5zqpybe5dfuhehtqdpsk6t54
* **Note:** Change the file name accordingly from the next step and add .tar.gz extension.
4. **Extract the Compressed Archive:**  Use the tar command to extract the downloaded .tar.gz archive. Type:
    ```bash
    tar -xvzf julia-1.9.2-linux-x86_64.tar.gz
5. **Copy the Extracted Folder:** Copy the extracted Julia folder to the /opt directory using the sudo cp command. Type:
    ```bash
    sudo cp -r julia-1.9.2 /opt/
6. **Create a Symbolic Link:** Create a symbolic link to the julia executable inside the /usr/local/bin folder. This allows you to run Julia from anywhere in the terminal. Use the sudo ln -s command:
    ```bash
    sudo ln -s /opt/julia-1.9.2/bin/julia /usr/local/bin/julia
7. **Test Installation:** Finally, you can test your Julia installation by opening a new terminal window and typing:
    ```bash
    julia
### Happy Coding!
---
Editor: Charan Madhu

