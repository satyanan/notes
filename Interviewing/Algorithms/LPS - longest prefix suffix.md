[leetcode tutorial](https://leetcode.com/problems/implement-strstr/discuss/13160/detailed-explanation-on-building-up-lps-for-kmp-algorithm)

``` c++
int i=0, j=1;
lps[0]=0;
while(j<W.length()){
	if(W[i] == W[j]){
		++i;
		lps[j]=i;
		++j;
	} else if(i==0){
		lps[j]=0;
		++j;
	}else{
		i = lps[i-1]
	}
}