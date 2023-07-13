# Comparing `tmp/dcentralab_qa_infra_automation-1.0.5.tar.gz` & `tmp/dcentralab_qa_infra_automation-1.0.6.tar.gz`

## Comparing `dcentralab_qa_infra_automation-1.0.5.tar` & `dcentralab_qa_infra_automation-1.0.6.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CreatePasswordPage.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/MetamaskInstallCompletedPage.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/.idea/workspace.xml` & `dcentralab_qa_infra_automation-1.0.6/.idea/workspace.xml`

 * *Files 23% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-1.0.5/.idea/workspace.xml` & `dcentralab_qa_infra_automation-1.0.6/.idea/workspace.xml`

```diff
@@ -2,14 +2,19 @@
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="ce720036-d8eb-462b-9d8d-e560b75fc3e8" name="Changes" comment="add infra developments">
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/__init__.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/data/read_data.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/data/read_data.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/BasePage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/BasePage.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-1.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-congratulations page
+successfully created wallet page
 
 @Author: Efrat Cohen
-@Date: 12.2022
+@Date: 06.2023
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'first-time-flow__header')]")
-ALL_DONE_BUTTON = (By.XPATH, "//*[contains(@class,'first-time-flow__button')]")
+TITLE = (By.XPATH, "//*[contains(@class, 'chakra-text css-h6dnxz')]")
+CLOSE_BTN = (By.XPATH, "//*[contains(@class, 'chakra-button css-1gr2my0')]")
 
 
-class CongratulationsPage(BasePage):
+class SuccessfullyCreatedWalletPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist("TITLE", TITLE)
 
-    def click_on_all_done(self):
+    def click_on_close_button(self):
         """
-        click on all done button
+        click on close button
         """
-        self.click("ALL_DONE_BUTTON", ALL_DONE_BUTTON)
+        self.click("CLOSE_BTN", CLOSE_BTN)
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-connect with metamask page
+congratulations page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'header__title')]")
-NEXT_BUTTON = (By.XPATH, "//*[contains(text(),'Next')]")
-CONNECT_BUTTON = (By.XPATH, "//button[contains(text(),'Connect')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Wallet creation successful')]")
+GOT_IT_BUTTON = (By.XPATH, "//*[contains(text(),'Got it')]")
 
 
-class ConnectWithMetamaskPage(BasePage):
+class CongratulationsPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist("TITLE", TITLE)
 
-    def click_on_next_button(self):
+    def click_on_got_it_button(self):
         """
-        click on next button
+        click on got it button
         """
-        self.click("NEXT_BUTTON", NEXT_BUTTON)
-
-    def click_on_connect_button(self):
-        """
-        click on connect button
-        """
-        self.click("CONNECT_BUTTON", CONNECT_BUTTON)
+        self.click("GOT_IT_BUTTON", GOT_IT_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 import wallet page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'first-time-flow__header')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Access your wallet')]")
 SECRET_RECOVERY_PHRASE_0 = (By.ID, "import-srp__srp-word-0")
 SECRET_RECOVERY_PHRASE_1 = (By.ID, "import-srp__srp-word-1")
 SECRET_RECOVERY_PHRASE_2 = (By.ID, "import-srp__srp-word-2")
 SECRET_RECOVERY_PHRASE_3 = (By.ID, "import-srp__srp-word-3")
 SECRET_RECOVERY_PHRASE_4 = (By.ID, "import-srp__srp-word-4")
 SECRET_RECOVERY_PHRASE_5 = (By.ID, "import-srp__srp-word-5")
 SECRET_RECOVERY_PHRASE_6 = (By.ID, "import-srp__srp-word-6")
 SECRET_RECOVERY_PHRASE_7 = (By.ID, "import-srp__srp-word-7")
 SECRET_RECOVERY_PHRASE_8 = (By.ID, "import-srp__srp-word-8")
 SECRET_RECOVERY_PHRASE_9 = (By.ID, "import-srp__srp-word-9")
 SECRET_RECOVERY_PHRASE_10 = (By.ID, "import-srp__srp-word-10")
 SECRET_RECOVERY_PHRASE_11 = (By.ID, "import-srp__srp-word-11")
-PASSWORD_INPUT = (By.ID, "password")
-CONFIRM_PASSWORD_INPUT = (By.ID, "confirm-password")
-AGREE_TERMS_CHECKBOX = (By.ID, "create-new-vault__terms-checkbox")
-SUBMIT_IMPORT_BUTTON = (By.XPATH, "//*[contains(@class,'submit-button')]")
+CONFIRM_BUTTON = (By.XPATH, "//*[contains(text(),'Confirm Secret Recovery Phrase')]")
 
 
 class ImportWalletPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
@@ -55,30 +52,12 @@
         self.enter_text("SECRET_RECOVERY_PHRASE_6", SECRET_RECOVERY_PHRASE_6, pytest.wallets_data.get("secret_recovery_phrase_6"))
         self.enter_text("SECRET_RECOVERY_PHRASE_7", SECRET_RECOVERY_PHRASE_7, pytest.wallets_data.get("secret_recovery_phrase_7"))
         self.enter_text("SECRET_RECOVERY_PHRASE_8", SECRET_RECOVERY_PHRASE_8, pytest.wallets_data.get("secret_recovery_phrase_8"))
         self.enter_text("SECRET_RECOVERY_PHRASE_9", SECRET_RECOVERY_PHRASE_9, pytest.wallets_data.get("secret_recovery_phrase_9"))
         self.enter_text("SECRET_RECOVERY_PHRASE_10", SECRET_RECOVERY_PHRASE_10, pytest.wallets_data.get("secret_recovery_phrase_10"))
         self.enter_text("SECRET_RECOVERY_PHRASE_11", SECRET_RECOVERY_PHRASE_11, pytest.wallets_data.get("secret_recovery_phrase_11"))
 
-    def insert_password(self):
+    def click_on_confirm(self):
         """
-        insert password
+        click on confirm button
         """
-        self.enter_text("PASSWORD_INPUT", PASSWORD_INPUT, pytest.wallets_data.get("password"))
-
-    def insert_confirm_password(self):
-        """
-        insert confirm password
-        """
-        self.enter_text("CONFIRM_PASSWORD_INPUT", CONFIRM_PASSWORD_INPUT, pytest.wallets_data.get("password"))
-
-    def agree_terms_of_use(self):
-        """
-        click on agree terms of use checkbox
-        """
-        self.click("AGREE_TERMS_CHECKBOX", AGREE_TERMS_CHECKBOX)
-
-    def click_on_submit_import_button(self):
-        """
-        click on import - submit the import form
-        """
-        self.click("SUBMIT_IMPORT_BUTTON", SUBMIT_IMPORT_BUTTON)
+        self.click("CONFIRM_BUTTON", CONFIRM_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 improve metamask page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'metametrics-opt-in__title')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Help us improve MetaMask')]")
 I_AGREE_BUTTON = (By.XPATH, "//*[contains(text(),'I agree')]")
 
 
 class ImproveMetamaskPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-new to metamask page
+allow the site to switch the network page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'select-action__body-header')]")
-IMPORT_WALLET_BUTTON = (By.XPATH, "//*[contains(text(),'Import wallet')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Allow this site to switch the network?')]")
+SWITCH_NETWORK_BUTTON = (By.XPATH, "//*[contains(text(),'Switch network')]")
 
 
-class NewToMetamaskPage(BasePage):
+class SwitchNetworkPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist("TITLE", TITLE)
 
-    def click_on_import_wallet(self):
+    def click_on_switch_network(self):
         """
-        click on import wallet
+        click on switch network button
         """
-        self.click("IMPORT_WALLET_BUTTON", IMPORT_WALLET_BUTTON)
+        self.click("SWITCH_NETWORK_BUTTON", SWITCH_NETWORK_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 welcome to metamask page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(text(),'Welcome to MetaMask')]")
-GET_STARTED_BUTTON = (By.XPATH, "//*[contains(text(),'Get started')]")
+TITLE = (By.XPATH, "//*[contains(text(),'get started')]")
+AGREE_TERMS_CHECKBOX = (By.ID, "onboarding__terms-checkbox")
+IMPORT_WALLET_BUTTON = (By.XPATH, "//*[contains(text(),'Import an existing wallet')]")
 CONNECT_WALLET_POPUP = (By.XPATH, "//*[contains(@class,'permissions-connect-header__title')]")
 
 
 class WelcomeToMetamaskPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
@@ -23,15 +24,21 @@
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist("TITLE", TITLE)
 
+    def click_on_agree_terms(self):
+        """
+        click on agree terms button
+        """
+        self.click("AGREE_TERMS_CHECKBOX", AGREE_TERMS_CHECKBOX)
+
     def is_button_exists(self):
-        return self.is_element_exist("GET_STARTED_BUTTON", GET_STARTED_BUTTON)
+        return self.is_element_exist("IMPORT_WALLET_BUTTON", IMPORT_WALLET_BUTTON)
 
-    def click_on_get_started(self):
+    def click_on_import_wallet(self):
         """
-        click on get started button
+        click on import wallet button
         """
-        self.click("GET_STARTED_BUTTON", GET_STARTED_BUTTON)
+        self.click("GET_STARTED_BUTTON", IMPORT_WALLET_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from dcentralab_qa_infra_automation.utils.WalletsActionsInterface import WalletsActionsInterface
 
 from dcentralab_qa_infra_automation.pages.metamaskPages.ConfirmPage import ConfirmPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.ImportWalletPage import ImportWalletPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.CongratulationsPage import CongratulationsPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.ConnectWithWalletPage import ConnectWithMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.ImproveMetamaskPage import ImproveMetamaskPage
-from dcentralab_qa_infra_automation.pages.metamaskPages.NewToMetamaskPage import NewToMetamaskPage
 from dcentralab_qa_infra_automation.pages.metamaskPages.SwitchNetworkPage import SwitchNetworkPage
-from dcentralab_qa_infra_automation.pages.metamaskPages.WalletConnectedHomePage import WalletConnectedHomePage
 from dcentralab_qa_infra_automation.pages.metamaskPages.WelcomeToMetamaskPage import WelcomeToMetamaskPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.CreatePasswordPage import CreatePasswordPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.MetamaskInstallCompletedPage import MetamaskInstallCompletedPage
 
 """
-coinbase wallet actions
+MetaMask wallet actions
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 
 class MetamaskActions(WalletsActionsInterface):
 
@@ -26,100 +26,123 @@
         self.driver = driver
 
     def import_wallet(self):
         """
         import wallet process
         """
         # Open new tab
-        # self.driver.execute_script("window.open('');")
+        self.driver.execute_script("window.open('');")
 
         # Focus on the new tab window
-        self.driver.switch_to.window(self.driver.window_handles[2])
+        self.driver.switch_to.window(self.driver.window_handles[1])
 
         # Open chrome extension
-        # self.driver.get(pytest.properties.get("metamask.connect.url"))
+        self.driver.get(pytest.properties.get("metamask.connect.url"))
 
         # Focus on the first tab window
-        # self.driver.switch_to.window(self.driver.window_handles[1])
+        self.driver.switch_to.window(self.driver.window_handles[1])
 
         welcomeToMetamaskPage = WelcomeToMetamaskPage(self.driver)
 
         # Check if metamask wallet page loaded
-        assert welcomeToMetamaskPage.is_page_loaded(), "welcome to metamask page loaded"
+        assert welcomeToMetamaskPage.is_page_loaded(), "Let's get started page loaded"
+
+        # Click on agree terms
+        welcomeToMetamaskPage.click_on_agree_terms()
 
         assert welcomeToMetamaskPage.is_button_exists()
 
-        # Click on get started button
-        welcomeToMetamaskPage.click_on_get_started()
+        # Click on import wallet button
+        welcomeToMetamaskPage.click_on_import_wallet()
 
         improveMetamaskPage = ImproveMetamaskPage(self.driver)
 
         # Check if improve to metamask page loaded
-        assert improveMetamaskPage.is_page_loaded(), "improve metamask page loaded"
+        assert improveMetamaskPage.is_page_loaded(), "Help us improve MetaMask page loaded"
 
         # Click on I agree button
         improveMetamaskPage.click_on_i_agree_button()
 
-        newToMetamaskPage = NewToMetamaskPage(self.driver)
-
-        # Check if new to metamask page loaded
-        assert newToMetamaskPage.is_page_loaded(), "new to metamask page loaded"
-
-        # Click on import wallet
-        newToMetamaskPage.click_on_import_wallet()
-
         importWalletPage = ImportWalletPage(self.driver)
 
         # Check if import wallet page loaded
-        assert importWalletPage.is_page_loaded(), "import wallet page loaded"
+        assert importWalletPage.is_page_loaded(), "Access your wallet with your Secret Recovery Phrase"
 
         # Insert secret recovery phrase
         importWalletPage.insert_secret_recovery_phrase()
 
+        # Click on confirm button
+        importWalletPage.click_on_confirm()
+
+        createPasswordPage = CreatePasswordPage(self.driver)
+
+        assert createPasswordPage.is_page_loaded(), "Create password page loaded"
+
         # Insert password
-        importWalletPage.insert_password()
+        createPasswordPage.insert_password()
 
         # Insert confirm password
-        importWalletPage.insert_confirm_password()
+        createPasswordPage.insert_confirm_password()
 
-        # Click on agree terms of use
-        importWalletPage.agree_terms_of_use()
+        # Click on understand MetaMask checkbox
+        createPasswordPage.click_on_understand_metamask_checkbox()
 
-        # Click on import button
-        importWalletPage.click_on_submit_import_button()
+        # Click on import wallet
+        createPasswordPage.click_on_import_wallet()
 
         congratulationsPage = CongratulationsPage(self.driver)
 
         # Check if congratulations page loaded
         assert congratulationsPage.is_page_loaded(), "congratulations page loaded"
 
-        # Click on all done button
-        congratulationsPage.click_on_all_done()
+        # Click on got it button
+        congratulationsPage.click_on_got_it_button()
+
+        metamaskInstallCompletedPage = MetamaskInstallCompletedPage(self.driver)
+
+        # Check if metamask install completed page loaded
+        assert metamaskInstallCompletedPage.is_page_loaded(), "metamask install completed page loaded"
 
-        walletConnectedHomePage = WalletConnectedHomePage(self.driver)
+        # Click on next button
+        metamaskInstallCompletedPage.click_on_next()
+
+        # Check is Done button exist
+        assert metamaskInstallCompletedPage.is_done_button_exist(), "Done button loaded"
+
+        # Click on Done button
+        metamaskInstallCompletedPage.click_on_done()
+
+        # Check is Try it out button exist
+        assert metamaskInstallCompletedPage.is_try_it_out_button_exist(), "Try it out button loaded"
 
-        # Check if wallet connected home page loaded
-        assert walletConnectedHomePage.is_page_loaded(), "wallet connected home page loaded"
+        # Click on Try it out button
+        metamaskInstallCompletedPage.click_on_try_it_out_button()
+
+        # Close Metamask tab
+        self.driver.close()
 
         # Focus on the new tab window
         self.driver.switch_to.window(self.driver.window_handles[0])
 
         time.sleep(2)
 
     def connect_wallet(self):
         """
         connect wallet implementation
         """
         time.sleep(3)
 
+        # Open new tab
+        self.driver.execute_script("window.open('');")
+
         # Switch focus to metamask tab
         self.driver.switch_to.window(self.driver.window_handles[1])
 
-        # Refresh the page
-        self.driver.refresh()
+        # Open chrome extension
+        self.driver.get(pytest.properties.get("metamask.connect.url"))
 
         connectWithMetamaskPage = ConnectWithMetamaskPage(self.driver)
 
         # Check if on connect with metamask page
         assert connectWithMetamaskPage.is_page_loaded(), "connect with metamask page loaded"
 
         # Click on next button
@@ -132,45 +155,41 @@
 
         # Check if switch network page loaded
         assert switchNetworkPage.is_page_loaded(), "allow site to switch the network page loaded"
 
         # Click on switch network button
         switchNetworkPage.click_on_switch_network()
 
-        walletConnectedHomePage = WalletConnectedHomePage(self.driver)
-
-        # Check if wallet connected home page loaded
-        assert walletConnectedHomePage.is_page_loaded(), "wallet connected home page loaded"
+        # Close MetaMask tab
+        self.driver.close()
 
         # Switch focus to site tab
         self.driver.switch_to.window(self.driver.window_handles[0])
 
     def confirm(self):
         """
         confirm wallet process
         """
         time.sleep(5)
 
+        # Open new tab
+        self.driver.execute_script("window.open('');")
+
         # Switch focus to metamask tab
         self.driver.switch_to.window(self.driver.window_handles[1])
 
-        # Refresh the page
-        self.driver.refresh()
+        # Open chrome extension
+        self.driver.get(pytest.properties.get("metamask.connect.url"))
 
         confirmPage = ConfirmPage(self.driver)
 
         # Check is confirm page loaded
         assert confirmPage.is_page_loaded(), "confirm page loaded"
 
         # Check is confirm button exist.
         assert confirmPage.is_confirm_button_exist()
 
         # Click on confirm button
         confirmPage.click_on_confirm_button()
 
-        walletConnectedHomePage = WalletConnectedHomePage(self.driver)
-
-        # Check if wallet connected home page loaded
-        assert walletConnectedHomePage.is_page_loaded(), "wallet connected home page loaded"
-
         # Switch focus to site tab
         self.driver.switch_to.window(self.driver.window_handles[0])
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py` & `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/LICENSE` & `dcentralab_qa_infra_automation-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.5/pyproject.toml` & `dcentralab_qa_infra_automation-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-1.0.5/PKG-INFO` & `dcentralab_qa_infra_automation-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 1.0.5
+Version: 1.0.6
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

