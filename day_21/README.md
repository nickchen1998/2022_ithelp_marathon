# Python 與自動化測試的敲門磚_Day21_CI/CD 簡介

每天的專案會同步到 github 上，可以前往 [這個網址](https://github.com/nickchen1998/2022_ithelp_marathon)
如果對於專案有興趣或是想討論一些問題，歡迎留言 OR 來信討論，信箱為：nickchen1998@gmail.com

## 一、CI/CD 簡介

CI/CD 其實是指兩個部分，分別是 Continuous Integration (持續整合) 以及 Continuous Deployment (持續部屬)，
下面我們就分別來進行說明。

- CI 持續整合
    
    在軟體開發的過程中，通常會由無數個開發人員一起工作，然而隨著程式碼以及人數的增加，專案會越來越難進行整合，
    這個時候我們就可以透過 CI 來進行。與其說 CI 是個工具，不如說 CI 是一種合作模式，藉由簡單的設定來讓 CI 工具替我們進行測試，
    就可以降低我們的專案在進行更新、整合時碰到問題的機率。

    在 CI，執行的過程中，會建議每個開發人員每天上班前先做一次 pull 的動作，於每天下班前至少執行一次 push 的動作，
    以此確保 CI 的運行效率。
    
- CD 持續部屬
    
    每當我們透過 CI 將專案整合完成後，便可以透過 CD 來進行自動化的部屬，減少我們在測試與部屬之間所耗費的時間

## 三、CI/CD 常用工具

- GitLab
  
  於 GitLab 上提供了 CI/CD 的介面，藉由在某處部屬好的 docker image，即可進行 CI/CD，為目前主流的 CI/CD 工具

- GitHub

  GitHub 於 2019 年推出了 GitHub Actions，此工具可以協助我們進行 CI，不過由於此功能還算新，尚有許多功能不成熟，
  因此比較建議使用在小型專案的 CI 當中

- Jenkins

  為目前主流的 CD 工具，藉由 GitLab 進行 CI 後，會將程式碼打包到 Jenkins 進行自動化部屬

## 四、內容預告

今天我們簡單介紹了 CI/CD 是什麼，就自動化測試這一塊來說，是比較著重再 CI (持續整合) 這塊，CD 的部分就牽扯到部屬的部分了，因此後面的進行
demo 的方向都會以 CI 的方向寫。

明天我們會花一天的時間介紹該如何在 Github 上使用 CI