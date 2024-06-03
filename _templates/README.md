# hygen

1. hygen 生成一个命令

   ```bash
   hygen generator new postName
   ```

2. 使用命令

   ```bash
   # 生成 postName new 下面所有文件
   hygen postName new

   # 生成 postName new 下面 aa 文件
   hygen postName new:aa

   # postName new 下有 prompt.js 的话，生成会提示输入内容
   module.exports = [
     {
       type: 'input',
       name: 'message',
       message: "What's your message?"
     }
   ]

   # 直接输入变量 --name 可以省略
   hygen postName new:aa --name 100

   # 帮助 help/index.ejs.t
   ---
   message: |
     hygen {bold generator new} --name [NAME] --action [ACTION]
     hygen {bold generator with-prompt} --name [NAME] --action [ACTION]
   ---

   ```
