偶然发现了一个练习 javascript 的 [代码库](https://github.com/kolodny/exercises)，发现那个外国人挺...，将题目的解答放在了 solutions 分支上面，题目放在 master 分支上面，然而他并没有告诉你解答放在 solutions 分支上面，并且当我发现有 solutions 分支的时候，竟然还发现代码被加密了... 

solutions 分支上面的 readme.md 文件内容：

    READ THIS FIRST
    
    Hello there, you seem to have quite an exploratory personality.
    Anyway if you found this place, you probably can figure out how to get to the solutions.
    Please don't publicize this branch, if people really want to know how to solve something then they'll find this themselves or ask someone else.

    If you do contribute a challenge, please also have a similar branch on your fork with a similar setup (some obscurity), although it isn't required.

果断的分析的一下，他竟然用同一段代码来进行解密和解码，实在是太神奇了。

在学习之前先来试验一下这段神奇的代码：

git clone 本仓库到本地，然后输入如下的命令，即可将代码进行加密和解密。

    →  ~/Learn/NodeJs_Practice/node_1 ✗✗✗ node code.js test.js 

效果的对比：

    //未加密的　test.js
    var test = function () {
        console.log('Hello World');
    });
    
    test();


    //加密后的 test.js
    '<+})8*)}`}7(/:)4./}ut}"
    }}}}:./*.18o1.6uvU811.}F.+19vtb
     tb
    
    )8*)utb


详细的知识点和原理分析，请访问我博客的链接 <http://spxiaomin.github.io/github_blog/nodejs/2015/10/11/nodejs-one.html>
