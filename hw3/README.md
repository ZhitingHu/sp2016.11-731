

 * `./decode` is the improved phrase-based decoder that allows reordering adjacent phrases
   - When translating phrase at position [i,j), we also consider the next phrase at 
     position [j,k), and add the reordered translation [j,k).english+trans[i,j).english 
     to stack[k]

 * `output.txt` is obtained by running
   
    ./decode -s 10 > output.txt
 
 * the score evaluated locally is -5229.566807
