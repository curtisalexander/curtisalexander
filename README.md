```bash
echo 'blah' | \
    tr 'ah' 'lo' | \
    sed -e 's/^[a-z]/H/' | \
    awk '{n=split($0,a,"");
        for (i in a) {if (a[i]=="H") print i " " a[i] "e";
        else print i " " a[i];} print n+1 " " "!"}' | \
    sort | \
    cut -d' ' -f2 | \
    paste -s -d '\0' -
```

### Projects

- [**ft**](https://github.com/curtisalexander/ft) — Fine-tuning explained, with a worked DistilBERT phone-number extraction example · [read the guide](https://curtisalexander.github.io/ft/)

<!--
**curtisalexander/curtisalexander** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
