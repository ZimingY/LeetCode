### 305.Number-of-Islands-II

本题的思想是，每遍历一个新陆地，默认count++。依次考察这个新陆地相邻的四块：如果相邻的是陆地，并且新陆地和老陆地的FindRoot不同，那么说明这是需要合并的两个集合，于是count--，并且将新陆地与旧陆地进行Union。最终实时输出count。