[tutorial](https://www.educative.io/edpresso/what-is-the-knuth-morris-pratt-algorithm)

Build lps table using [[LPS - longest prefix suffix]]


```


``` c++
# Initialising variables:i = 0j = 0m = len(W)n = len(S)# Start search:while (i < m && j < n){    # Last character matches -> Substring found:    if (W[i] == S[j] && i == m - 1):        return true    # Character matches:    else if (W[i] == S[j]):        i++        j++        # Character didn't match -> Backtrack:    else:        i = arr[i - 1]        if i == 0:            j++}# Substring not found:return false
```
