# runpython
測試能否將 Brython 編輯器放在 Github Pages 然後執行結果顯示在另一個瀏覽器視窗 (無法達到目的)

Github Pages: https://mdecourse.github.io/runpython/

由於 Github Pages 只是一個能夠支援 Javascript 在近端執行的靜態全球資訊網系統, 因此沒有 ajax 的機制.

將 Brython-server 架在一般 Ubuntu 主機時, 可以透過 redis 儲存 session, 可以透過系統變數存放 Github API 的相關設定私密檔案, 可以啟用 Github API 帳號登入, 可以直接在線上編輯特定檔案後提交推送改版.

但是採用 Github Pages 之後, 只剩下可以執行 Brython 程式, 但是嘗試 windows.open().document.write() 不會開新視窗, 而是在原始的 index.html 視窗中執行.


