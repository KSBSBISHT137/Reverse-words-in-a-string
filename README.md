# Reverse-words-in-a-string
Code for reverse a words in a string

 string reverseWords(string S) {
        string res="",s="";
        for(int i=0;i<S.size();i++) {
            while(S[i]!='.' and i<S.size()) {
                s+=S[i++];
            }
            res.insert(0,s);
            res.insert(0,".");
            s="";
        }
        res.erase(res.begin()+0);
        return res;
    } ;
