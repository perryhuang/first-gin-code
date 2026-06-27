1. 建立一個Agent一直不斷監視使用者如何使用電腦. 並對使用者問目前在做甚麼事. 
2. 使用者可以一面做自己的事, 一面用語音回答Agent. 教Agent目前做的事的目的. Agent自發把從使用者身上學會的知識轉成.md 檔. 當做未來Agent自主做事的手冊.
3.



主Agent指派多個sub-Agent工作.  (Detail about subAgent: https://code.claude.com/docs/zh-TW/plugins-reference)
主Agent:
CLAUDE.md - 鐉寫各種不同的sub-Agent所需要的不同CLAUDE.md的技能. 

Example:

Workspace 
   |--------- CLAUDE.md (指派工作技能的MD file) 主Agent裡的CLAUDE.md 
   |          內容說明SubAgentClaudeMd資料夾中各種不同的XXXXXXX-CLAUDE.md, 
   |          會因指派的任務不同copy XXXX-CLAUDE.md 到新建任務的資料夾. 
   |          並到xxxx-claude.md copy到該新建資料夾並命名成CLAUDE.md
   |
   |--------- <SubAgentClaudeMd>
   |                  |---- WIKI-CLAUDE.MD
   |                  |---- CODE-CLAUDE.MD (andrej-karpathy-skills CLAUDE.MD)
   |                  |---- VERIFY-CLAUDE.MD (驗證 CLAUDE.MD)
   |
   |
   |--------> <WIKI FOLDER>   (New create by Major Agent)
   |--------> <CODE FOLDER>   (New create by Major Agent)
   |--------> <VERIFY FOLDER> (New create by Major Agent)

