# Info
This class library project lets you to get System,Software,AntiProducts,FireWall,Browsing and Network Info

            SystemDetail systemDetail = new SystemDetail();
            var systeminfo = systemDetail.getSystemInfo();//Get Hardware and Operating System info
            var userDetails=systemDetail.getUserDetails(); //Get User Detail 
            var updates=systemDetail.getWindowsUpdate();//Get Installed Updates Details 
            var windowServices = systemDetail.getWindowServices();//get Installed Windows Services Details
            var groups = systemDetail.getGroups();//get Details of Groups on Windows 
            var drives = systemDetail.getDriverInfo();//get Drives Info
            var drivers = systemDetail.GetDrivesInfo();//get Drives Info Info
            
            GoogleChrome chrome = new GoogleChrome();
            var chromeHistory = chrome.GetHistory();//Get Chrome Browser History

            Firefox firefox = new Firefox();
            var firefoxHistory = firefox.GetHistory();//Get FireFox Browser History

            InternetExplorer ie = new InternetExplorer();
            var ieHistory = ie.GetHistory();//Get IE Browser History

            Browsers browser = new Browsers();
            List<String> browsers=browser.getBrowsers();//get Installed Browser List 
            browser.blocksite("http://google.com");//Block Site on System
            browser.unblocksite("http://google.com");//UnBlock Site on System

            Activites activites = new Activites();
            var applicationlogs=activites.getEventLogs("Application");//get Events Logs 
            var recenttDirectories = activites.GetRecentDirectories();
            var process = activites.GetProcesses();
