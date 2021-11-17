# pascals-triangle-1
class Solution { public:     vector&lt;vector&lt;int>> generate(int numRows) {         vector&lt;vector&lt;int>>ans;         for(int i=0;i&lt;numRows;i++){             vector&lt;int>row(i+1,1);             for(int j=1;j&lt;i;j++)             {                 row[j]=ans[i-1][j]+ans[i-1][j-1];             }             ans.push_back(row);         }         return ans;     } };
