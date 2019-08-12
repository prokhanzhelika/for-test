<?xml version="1.0" encoding="windows-1251"?>
<configuration>
  <params>
      <param name="VoiceControl" description="Голосовое управление в мобильном приложении">
           <type>list</type>ER
           <enabled>true</enabled>
           <nodes>
              <node id="node0.online.sberbank.ru">
                 <search>true</search>
                 <search10.0>false</search10.0>
              </node>
              <node id="node1.online.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
              <node id="node2.online.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
              <node id="node3.online.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
              <node id="greenfield1.online.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
              <node id="mobile.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
              <node id="ift-node1.testonline.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
              <node id="ift-node2.testonline.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
              </node>
             <node id="greenfield2.online.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
             </node>
             <node id="ift-node1-mp.testonline.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
             </node>
             <node id="ift-node2-mp.testonline.sberbank.ru">
                 <search>false</search>
                 <search10.0>true</search10.0>
             </node>
         </nodes>
      </param>
        <param name="SmartSearchTransfer" description="Умный поиск">
                 <type>setting</type>
                 <enabled>true</enabled>
          <nodes>
          <node id="mobile.sberbank.ru">
                 <enabled>true</enabled>
              </node>
          </nodes>
  </param>
        <param name="OptimalAccountTransferWithMaskCheck" description="Оптимизированный перевод на счет клиенту Сбербанка">
            <enabled>true</enabled>
            <masksEnabled>true</masksEnabled>
            <maskTutorialEnabled>true</maskTutorialEnabled>
            <accountsMaskCollection>
            	<accountsMask paymentSystem="unavailable">
                  	<mask>^([0-9]{5})(([^8][0-9]{2})|(8[^1][0-9])|(81[^0]))([0-9]{11,})</mask>
              	</accountsMask>
            	<accountsMask paymentSystem="P2B">
                	<mask>^(40)([1-7])([0-9]{2})(810)([0-9]{11,})</mask>
                	<mask>^(4080)([2457])(810)([0-9]{11,})</mask>
              	</accountsMask>
			</accountsMaskCollection>
      	</param>
      	<param name="SecuritySettings" description="Настройки безопасности под кнопкой Безопасность">
 			<type>setting</type> 
    		<enabled>true</enabled>
 			<nodes>
  				<node id="node0.online.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="node1.online.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="node2.online.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="node3.online.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="node4.online.sberbank.ru">
     				<enabled>false</enabled>
   				<node id="greenfield1.online.sberbank.ru">
  				</node>
     				<enabled>false</enabled>
  				</node>
   				<node id="greenfield2.online.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="mobile.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="ift-node1.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="ift-node2.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
              	<node id="ift-node3.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
              	<node id="ift-node4.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="ift-node1-mp.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="ift-node2-mp.testonline.sberbank.ru">
     				<enabled>true</enabled>
  				</node>
              	<node id="ift-node3-mp.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
              	<node id="ift-node4-mp.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="psinode2.testonline.sberbank.ru">
    				<enabled>false</enabled>
  				</node>
   				<node id="psinode1.testonline.sberbank.ru">
     				<enabled>false</enabled>
  				</node>
   				<node id="194.186.207.23">
     				<enabled>false</enabled>
  				</node>
 			</nodes>
      </param>
		<param name="TransferMIRExternal" description="Переводы на карты МИР сторонних банков">
     		<enabled>true</enabled>
     		<type>setting</type>
     		<buttonToMessenger>true</buttonToMessenger>
		</param>
          	<param name="BetaFeatures" description="Функционал для бета-версии СБОЛа">
     		<enabled>true</enabled>
     		<type>setting</type>
     		<buttonToMessenger>false</buttonToMessenger>
		</param>
		<param name="PrintAutoTransferCheck" description="Печать чека по совершённому автопереводу в выписке операций">
          	<type>setting</type>
     		<enabled>true</enabled>
		</param>
		<param name="OnDemandDeeplink" description="Диплинк в процесс создания переводов любому человеку">
          	<type>setting</type>
     		<enabled>true</enabled>
		</param>
      	<param name="SberKids" description="Родительский функционал СберKids">
          <eribMarkers>false</eribMarkers>
          <offers>true</offers>
          <sberKidsAvailable>true</sberKidsAvailable>         
        </param>
    	<param name="CreditReportService" description="Отчет о кредитной истории">
			<type>setting</type>
			<enabled>true</enabled>
			<creditReportServiceTutorialEnabled>true</creditReportServiceTutorialEnabled>
          	<creditReportServiceGetpdfEnabled>true</creditReportServiceGetpdfEnabled>
          	<creditReportServiceDeeplinkEnabled>true</creditReportServiceDeeplinkEnabled>
		</param>
      	<param name="SberRatingService" description="Сбербанк рейтинг">
			<type>setting</type>
			<enabled>false</enabled>
          	<sberRatingServiceDeeplinkEnabled>true</sberRatingServiceDeeplinkEnabled>
		</param>
      	<param name="PriorityCardP2PServiceWrongCardsExclude" description="Исключение карт с истекшим сроком действия из списка карт, которые можно выбрать приоритетной">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
    <param name="InternalTransfersRoutes" description="На карту или счет в другой банк из МСС">
		<type>setting</type>
		<enabled>true</enabled>
	</param>
    <param name="paymentDeduplicateServiceProvider" description="Исключение дублей при поиске услуг">
		<type>setting</type>
		<enabled>true</enabled>
	</param>
    <param name="HideCreditCard" description="Исключение кредитной карты из раздела приоритетная карта">
		<type>setting</type>
		<enabled>true</enabled>
	</param>
    <param name="CardCheckLuhn" description="  Функционал проверки номера карты по алгоритму Луна в классических переводах по номеру карты">
      <type>setting</type>
      <enabled>false</enabled>
    </param>
      	<param name="TransfersPostcard" description="Прикрепление открытки в p2p переводах">
        	<type>setting</type>
            <enabled>true</enabled>
        </param> 
      <param name="AUPAutorepaymentTutorial" description="Таргер тап Автопогашение">
        <type>setting</type>
        <enabled>true</enabled>
        <nodes>
            <node id="node0.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
                <enabled>true</enabled>
            </node>
            <node id="ift-node0-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
                <enabled>true</enabled>
            </node>
            <node id="mobile.sberbank.ru" description="Стенд ПСИ">
                <enabled>true</enabled>
            </node>
        </nodes>
    </param>

      	<param name="Loyalty" description="Программа лояльности «Спасибо от Сбербанка»">
			<type>list</type>
			<enabled>true</enabled>
          	<partnerDistanceSettings>
              <enabled>true</enabled>
              <showDistance>true</showDistance>
              <minimumSignificantDistanceInMeters>10</minimumSignificantDistanceInMeters>
              <valueInMetersWhenWeStartUsingKilometers>1000</valueInMetersWhenWeStartUsingKilometers>
              <maximumSignificantDistanceInKilometers>10</maximumSignificantDistanceInKilometers>
              <DeepLinkSpasibo>true</DeepLinkSpasibo>
            </partnerDistanceSettings>
			<nodes>
				<node id="mobile.sberbank.ru" description="Стенд ПСИ">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
                <node id="ift-node1.testonline.sberbank.ru" description="Стенд ИФТ блок 1">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
                <node id="ift-node2.testonline.sberbank.ru" description="Стенд ИФТ блок 2">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
                <node id="ift-node3-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 3 (мобильный)">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
                <node id="ift-node4-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 4 (мобильный)">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
                <node id="ift-node5-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 5 (мобильный)">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                </node>
           	    <node id="ift-node0-mp.testonline.sberbank.ru" description="Стенд ИФТ блок Stand-In (мобильный)">
                    <bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <useLottieLoader>true</useLottieLoader>
                </node>
				<node id="node0.online.sberbank.ru">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
				<node id="node1.online.sberbank.ru">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
				<node id="node2.online.sberbank.ru">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
				<node id="node3.online.sberbank.ru">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
				<node id="node4.online.sberbank.ru">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<bonusBalance>true</bonusBalance>
					<dashboard>true</dashboard>
					<offers>true</offers>
                    <charityPLSpasibo>true</charityPLSpasibo>
                    <distanceToNearestSalesPoint>true</distanceToNearestSalesPoint>
                    <ClientPrivilegeLevel>true</ClientPrivilegeLevel>
                    <ClientPrivilegeLevelNew>true</ClientPrivilegeLevelNew>
                  	<LoyaltyUICorrectionsEnabled>true</LoyaltyUICorrectionsEnabled>
                    <SearchLoyalty>true</SearchLoyalty>
                    <useLottieLoader>true</useLottieLoader>
                    <DeepLinkSpasibo>true</DeepLinkSpasibo>
                    <CardSelectSpasibo>true</CardSelectSpasibo>
				</node>
			</nodes>
		</param>
        <param name="LoyaltyPreloginZone" description="Прелогин зона Спасибо">
            <type>list</type>
			<enabled>true</enabled>
        </param>
	    <param name="Premier" description="Функционал Сбербанк Пресмьер">
			<type>list</type>
	 		<nodes>
                 <node id="mobile.sberbank.ru" description="Стенд ПСИ">
                     <distanceMarking>true</distanceMarking>
                     <meetingListScreen>true</meetingListScreen>
                     <createMeeting>true</createMeeting>
                </node>
                <node id="ift-node1.testonline.sberbank.ru" description="Стенд ИФТ блок 1">
                     <distanceMarking>true</distanceMarking>
                     <meetingListScreen>true</meetingListScreen>
                     <createMeeting>true</createMeeting>
                </node>
                <node id="ift-node2.testonline.sberbank.ru" description="Стенд ИФТ блок 2">
                     <distanceMarking>true</distanceMarking>
                     <meetingListScreen>true</meetingListScreen>
                     <createMeeting>true</createMeeting>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
                     <distanceMarking>true</distanceMarking>
                     <meetingListScreen>true</meetingListScreen>
                     <createMeeting>true</createMeeting>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
                     <distanceMarking>true</distanceMarking>
                     <meetingListScreen>true</meetingListScreen>
                     <createMeeting>true</createMeeting>
                </node>
                <node id="ift-node0-mp.testonline.sberbank.ru" description="Стенд ИФТ блок Stand-In (мобильный)">
                     <distanceMarking>true</distanceMarking>
                     <meetingListScreen>true</meetingListScreen>
                     <createMeeting>true</createMeeting>
                </node>
			</nodes>
		</param>
        <param name="RecommendedDebt" description="Смарт Счета">
          <type>service</type>
          <enabled>true</enabled>
          <createAutoPayment>false</createAutoPayment>
          <providerViewFlexibleNavBar>false</providerViewFlexibleNavBar>
          <nodes>
          	<node id="mobile.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
                <providerChips>true</providerChips>
                <offRefactor>true</offRefactor>
                <offRefactor_v912>false</offRefactor_v912>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="ift-node2-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
          	<node id="ift-node4-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
          	<node id="ift-node5-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
            <node id="ift-node7-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
            <node id="ift-node8-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>false</providerViewFlexibleNavBar>
                <createAutoPayment>false</createAutoPayment>
			</node>
			<node id="ift-node0-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
  			</node>
			<node id="node0.online.sberbank.ru">
				<enabled>false</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>false</paymentService_v96>
				<debtService>false</debtService>
             	<debtRemoveService>false</debtRemoveService>
				<debtRenameService>false</debtRenameService>
                <providerChips>false</providerChips>
                <createAutoPayment>false</createAutoPayment>
			</node>
			<node id="node1.online.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>false</debtService>
             	<debtRemoveService>false</debtRemoveService>
				<debtRenameService>false</debtRenameService>
                <providerChips>true</providerChips>
                <offRefactor>true</offRefactor>
                <offRefactor_v912>false</offRefactor_v912>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="node2.online.sberbank.ru">
				<enabled>false</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>false</paymentService_v96>
				<debtService>false</debtService>
             	<debtRemoveService>false</debtRemoveService>
				<debtRenameService>false</debtRenameService>
                <providerChips>true</providerChips>
                <createAutoPayment>false</createAutoPayment>
			</node>
			<node id="node3.online.sberbank.ru">
				<enabled>false</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>false</paymentService_v96>
				<debtService>false</debtService>
             	<debtRemoveService>false</debtRemoveService>
				<debtRenameService>false</debtRenameService>
                <providerChips>false</providerChips>
                <createAutoPayment>false</createAutoPayment>
			</node>
			<node id="node4.online.sberbank.ru">
				<enabled>false</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>false</paymentService_v96>
				<debtService>false</debtService>
             	<debtRemoveService>false</debtRemoveService>
				<debtRenameService>false</debtRenameService>
                <providerChips>false</providerChips>
                <createAutoPayment>false</createAutoPayment>
			</node>
			<node id="greenfield1.online.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
                <providerChips>true</providerChips>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="greenfield2.online.sberbank.ru">
				<enabled>false</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>false</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
                <providerChips>true</providerChips>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="ift-node1.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
                <providerChips>false</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="ift-node2.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
                <providerChips>true</providerChips>
                <offRefactor>false</offRefactor>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
          	<node id="ift-node4.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
          	<node id="ift-node5.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
            <node id="ift-node7.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <offRefactor>true</offRefactor>
                <offRefactor_v912>false</offRefactor_v912>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
            <node id="ift-node8.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
              	<paymentService_v96>true</paymentService_v96>
				<debtService>true</debtService>
             	<debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>true</providerChips>
                <offRefactor>true</offRefactor>
                <offRefactor_v912>false</offRefactor_v912>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
            <node id="psinode2.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>false</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="psinode1.testonline.sberbank.ru">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>false</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
			<node id="194.186.207.23">
				<enabled>true</enabled>
				<paymentService>false</paymentService>
             	<paymentService_v96>true</paymentService_v96>
              	<debtService>true</debtService>
                <debtRemoveService>true</debtRemoveService>
				<debtRenameService>true</debtRenameService>
              	<providerChips>false</providerChips>
                <providerViewFlexibleNavBar>true</providerViewFlexibleNavBar>
                <createAutoPayment>true</createAutoPayment>
			</node>
		</nodes>
	</param>     	
    <param name="DeepLinkeInvoicingPayment" description="Диплинк для инициации биллингового платежа из МП ПУ (v2)">
    	<type>list</type>
		<enabled>true</enabled>
		<providers>
          	<provider name="ТСЖ Малкова" codeservice="560523"/>
            <provider name="Система Город, Челябинская область" codeservice="366286825102"/>
            <provider name="Система Город Алтайского края" codeservice="118436920413"/>
            <provider name="inDriver" codeservice="282031456838"/>
            <provider name="Иркутскэнергосбыт (эл.энергия)" codeservice="19759901572"/>
            <provider name="Иркутскэнерго (тепло)" codeservice="55090486690"/>
            <provider name="Служба эксплуатации" codeservice="449240516721"/>
            <provider name="ВГМУ им. Н. Н. Бурденко" codeservice="252289179937"/>
            <provider name="ГК F5" codeservice="350593254756"/>
            <provider name="ГК F5" codeservice="350620523517"/>
            <provider name="ГК F5" codeservice="350671407229"/>
            <provider name="НТВ-Плюс" codeservice="193183284635"/>
            <provider name="Уфанет" codeservice="372440012900"/>
		</providers>
    	<nodes>
			<node id="ift-node1-mp.testonline.sberbank.ru">
              <enabled>true</enabled>
			</node>
			<node id="ift-node2-mp.testonline.sberbank.ru">
              <enabled>true</enabled>
			</node>
			<node id="ift-node5-mp.testonline.sberbank.ru">
              <enabled>true</enabled>
			</node>
			<node id="greenfield1.online.sberbank.ru">
              <enabled>false</enabled>
			</node>
			<node id="node1.online.sberbank.ru">
              <enabled>true</enabled>
			</node>
			<node id="node2.online.sberbank.ru">
              <enabled>true</enabled>
			</node>
			<node id="node3.online.sberbank.ru">
              <enabled>true</enabled>
			</node>
			<node id="node4.online.sberbank.ru">
              <enabled>true</enabled>
			</node>
		</nodes>
	</param>
    <param name="DebitCardExtraTips" description="Расширенные текстовки для трекинга доставки карт">
    <type>service</type>
    <enabled>true</enabled>
    <nodes>
        <node id="node0.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="node4.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="greenfield2.online.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="mobile.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node1.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node2.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node3.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node4.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node4-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node5-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="ift-node7-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="psinode2.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="psinode1.testonline.sberbank.ru">
            <enabled>true</enabled>
        </node>
        <node id="194.186.207.23">
            <enabled>true</enabled>
        </node>
    </nodes>
	</param>
	<param name="needRqDeliveryStatus" description="Анализ статуса доставки активированных карт">
        <type>service</type>
        <enabled>true</enabled>
        <nodes>
            <node id="node0.online.sberbank.ru">
                <enabled>false</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
                <enabled>false</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
                <enabled>false</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
                <enabled>false</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
                <enabled>false</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="mobile.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node3.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node7-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="194.186.207.23">
                <enabled>true</enabled>
            </node>
        </nodes>
	</param>
	<param name="ActivationCardClaim" description="Активация дебетовых карт">
        <type>service</type>
        <enabled>false</enabled>
        <tutorial>true</tutorial>
		<usl_card2_reference>http://www.sberbank.ru/common/img/uploaded/files/pdf/usl_card2.pdf</usl_card2_reference>
        <nodes>
            <node id="node0.online.sberbank.ru">
                <enabled>false</enabled>
                <tutorial>false</tutorial>
            </node>
            <node id="node1.online.sberbank.ru">
                <enabled>false</enabled>
                <tutorial>false</tutorial>
            </node>
            <node id="node2.online.sberbank.ru">
                <enabled>false</enabled>
                <tutorial>false</tutorial>
            </node>
            <node id="node3.online.sberbank.ru">
                <enabled>false</enabled>
                <tutorial>false</tutorial>
            </node>
            <node id="node4.online.sberbank.ru">
                <enabled>false</enabled>
                <tutorial>false</tutorial>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
           	<node id="psinode1.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="mobile.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
           	<node id="ift-node1.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node3.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node4.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
            <node id="ift-node4-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
                <tutorial>true</tutorial>
			</node>
			<node id="ift-node5-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
                <tutorial>true</tutorial>
			</node>
			<node id="ift-node7-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
                <tutorial>true</tutorial>
			</node>
            <node id="194.186.207.23">
                <enabled>true</enabled>
                <tutorial>true</tutorial>
            </node>
        </nodes>
	</param>
    <param name="RenovatedTargetCreation" description="Создание цели в новом дизайне">
      	<nodes>
            <node id="node0.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
           	<node id="psinode1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="mobile.sberbank.ru">
                <enabled>true</enabled>
            </node>
           	<node id="ift-node1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node3.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node5-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node7-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
            <node id="194.186.207.23">
                <enabled>true</enabled>
            </node>
        </nodes>
	</param>
	<param name="DebitCardAppMP" description="Заказ дебетовых карт">
		<type>service</type>
		<enabled>true</enabled>
      	<enabled_8_7>true</enabled_8_7>
		<digitalcardshow>true</digitalcardshow>
      	<ikaotransliteration>false</ikaotransliteration>
      	<apiv2>true</apiv2>
      	<api_urls>
			<api_url name="searchBranches_v1" url="/card/v1/mobile/rest/searchBranches"/>
			<api_url name="searchBranches_v2" url="/card/v2/mobile/rest/searchBranches"/>
			<api_url name="init_v1" url="/card/v1/mobile/rest/init"/>
			<api_url name="init_v2" url="/card/v2/mobile/rest/init"/>
			<api_url name="create_v1" url="/card/v1/mobile/rest/create"/>
			<api_url name="create_v2" url="/card/v2/mobile/rest/create"/>
			<api_url name="send_v1" url="/card/v1/mobile/rest/send"/>
			<api_url name="send_v2" url="/card/v2/mobile/rest/send"/>
			<api_url name="operationHistory_v1" url="/card/v1/mobile/rest/OperationHistory"/>
			<api_url name="operationHistory_v2" url="/card/v2/mobile/rest/OperationHistory"/>
			<api_url name="countries_v1" url="/card/v1/mobile/rest/countries"/>
			<api_url name="countries_v2" url="/card/v2/mobile/rest/countries"/>
    	</api_urls>
		<nodes>
			<node id="node0.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>false</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>false</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="node1.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>false</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>false</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="node2.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>false</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>false</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="node3.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>false</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>false</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="node4.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>false</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>false</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="greenfield1.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="greenfield2.online.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="mobile.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="ift-node1.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="ift-node2.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
            <node id="ift-node7.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="ift-node0-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="ift-node1-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="ift-node2-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
            <node id="ift-node7-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="psinode2.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="psinode1.testonline.sberbank.ru">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
			<node id="194.186.207.23">
				<enabled>true</enabled>
              	<apiv2>true</apiv2>
				<fatkashow>false</fatkashow>
				<ufsbranches>true</ufsbranches>
				<ufshistory>true</ufshistory>
				<digitalcardshow>true</digitalcardshow>
              	<ikaotransliteration>false</ikaotransliteration>
			</node>
		</nodes>
	</param>
	<param name="DigitalCardAppMP" description="Заказ цифровых карт">
		<type>service</type>
      	<embossingtitle>Имя владельца</embossingtitle>
    	<embossingvalue>DIGITAL CARD</embossingvalue>
    	<embossingdescription>Это поле может пригодиться для оплаты в интернете</embossingdescription>
        <enabled>true</enabled>
        <ufshistory>true</ufshistory>
        <classic-encryption>true</classic-encryption>
		<nodes>
			<node id="node0.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <showhints>true</showhints>
			</node>
			<node id="node1.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <showhints>true</showhints>
			</node>
			<node id="node2.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <showhints>true</showhints>
			</node>
			<node id="node3.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <showhints>true</showhints>
			</node>
			<node id="node4.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <showhints>true</showhints>
			</node>
			<node id="greenfield1.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panrq>true</panrq>
                <showhints>true</showhints>         
			</node>
			<node id="greenfield2.online.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panrq>true</panrq>
                <showhints>true</showhints>              
			</node>
			<node id="mobile.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panrq>true</panrq>
                <showhints>true</showhints>
			</node>
			<node id="ift-node1-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panrq>true</panrq>
                <showhints>true</showhints>
			</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panrq>true</panrq>
                <showhints>true</showhints>
			</node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panmask>true</panmask>
                <panrq>true</panrq>
                <classic-encryption>true</classic-encryption>
				<tutor>true</tutor>
			</node>
          <node id="ift-node7-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panmask>true</panmask>
                <panrq>true</panrq>
                <classic-encryption>true</classic-encryption>
				<tutor>true</tutor>
			</node>
          <node id="ift-node0-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panmask>true</panmask>
                <panrq>true</panrq>
                <classic-encryption>true</classic-encryption>
				<tutor>true</tutor>
			</node>
          <node id="psinode1.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panmask>true</panmask>
                <panrq>true</panrq>
                <classic-encryption>true</classic-encryption>
				<tutor>true</tutor>
			</node>
          <node id="psinode2.testonline.sberbank.ru">
				<enabled>true</enabled>
				<fatkashow>false</fatkashow>
				<getcvv>true</getcvv>
				<ufshistory>true</ufshistory>
                <blocknotification>true</blocknotification>
              	<embossingenabled>true</embossingenabled>
                <panmask>true</panmask>
                <panrq>true</panrq>
                <classic-encryption>true</classic-encryption>
				<tutor>true</tutor>
			</node>
		</nodes>
		</param> 
        <param name="CardPANRequest" description="Определение типов карт для которых доступен запрос полного номера карты">
        	<type>service</type>
            <enabled>true</enabled>
			<CardPANRqList>
                <CardPANRq id="MasterCard Mass"/>   
				<CardPANRq id="Visa Classic"/>
                <CardPANRq id="Visa Digital"/>
			 	<CardPANRq id="Visa Platinum"/>                                         
                <CardPANRq id="MIR Gold"/>
                <CardPANRq id="MasterCard Business Digital"/>
                <CardPANRq id="Visa Business Digital"/>
                <CardPANRq id="MasterCard World Elite Sberbank1"/>
                <CardPANRq id="MasterCard World Black Edition PREMIER"/>
              	<CardPANRq id="World MasterCard 'Золотой'"/>
                <CardPANRq id="Visa Gold 'Золотой'"/>
			</CardPANRqList>
      </param>
        <param name="CardPANRq" description="Определение типов карт для запроса PAN-номера карты">
			<type>list</type>
			<enabled>true</enabled>
			<key>name</key>
			<CardPANRqList>
              	<CardPANRq id="Visa Classic"/>
                <CardPANRq id="Visa Gold"/>
                <CardPANRq id="Visa Digital"/>
                <CardPANRq id="MIR"/>
				<CardPANRq id="Visa Platinum"/>
				<CardPANRq id="MasterCard Gold"/>
                <CardPANRq id="Visa Virtual"/>
                <CardPANRq id="MasterCard Business Digital"/>
                <CardPANRq id="Visa Business Digital"/>
                <CardPANRq id="MasterCard World Elite Sberbank1"/>
                <CardPANRq id="Visa Gold 'Золотой'"/>
              	<CardPANRq id="World MasterCard 'Золотой'"/>
                <CardPANRq id="MasterCard World Black Edition PREMIER"/>
			</CardPANRqList>
		</param>
        <param name="CardCVVSMS" description="Определение типов карт для которых доступен запрос CVC2/CVV2">
			<type>service</type>
            <enabled>true</enabled>            
			<cardCvvList>		
                <cardCvv id="MasterCard World Elite Sberbank1"/>
                <cardCvv id="MasterCard World Black Edition PREMIER"/>
                <cardCvv id="MasterCard Mass"/>
                <cardCvv id="Visa Digital"/>
                <cardCvv id="Visa Virtual"/>
                <cardCvv id="Visa Platinum"/>
              	<cardCvv id="MasterCard Platinum"/>
                <cardCvv id="Visa Classic Бесконтактная"/>
                <cardCvv id="MIR Gold"/>
                <cardCvv id="MIR Premium"/>
                <cardCvv id="МИР Momentum"/>
                <cardCvv id="MIR Momentum"/>
                <cardCvv id="Visa Infinite"/>                
                <cardCvv id="Visa Platinum PREMIER"/>
                <cardCvv id="Visa Signature"/>
                <cardCvv id="MIR Premium Plus"/> 
                <cardCvv id="Visa Gold"/>
                <cardCvv id="Electron"/>                
                <cardCvv id="Visa Classic"/>
                <cardCvv id="MasterCard Standard Бесконтактная"/> 
                <cardCvv id="Visa Infinite Sberbank1"/>
              	<cardCvv id="World MasterCard 'Золотой'"/>
              	<cardCvv id="Visa Gold 'Золотой'"/>
			</cardCvvList>
		</param>
		<param name="CardCVV" description="Определение типов карт для запроса CVV">
			<type>list</type>
			<enabled>true</enabled>
			<key>name</key>
			<cardCvvList>
              	<cardCvv id="Visa Classic"/>
                <cardCvv id="MasterCard World Elite Sberbank1"/>
                <cardCvv id="MasterCard World Black Edition PREMIER"/>
                <cardCvv id="Visa Virtual"/>
                <cardCvv id="Visa Digital"/>
                <cardCvv id="Visa Platinum"/>
              	<cardCvv id="MasterCard Platinum"/>
                <cardCvv id="Visa Classic Бесконтактная"/>
                <cardCvv id="MIR"/>
                <cardCvv id="MIR Gold"/>
                <cardCvv id="MIR Premium"/>
                <cardCvv id="МИР Momentum"/>
                <cardCvv id="MIR Momentum"/>
                <cardCvv id="Visa Infinite"/>                
                <cardCvv id="Visa Platinum PREMIER"/>
                <cardCvv id="Visa Signature"/>
                <cardCvv id="MIR Premium Plus"/> 
                <cardCvv id="Visa Gold"/>
                <cardCvv id="Electron"/>
                <cardCvv id="MasterCard Gold"/>
                <cardCvv id="MasterCard Standard Бесконтактная"/> 
                <cardCvv id="Visa Infinite Sberbank1"/>
              	<cardCvv id="World MasterCard 'Золотой'"/>
              	<cardCvv id="Visa Gold 'Золотой'"/>
			</cardCvvList>
		</param>
        <param name="CardPANMask" description="Определение типов карт для маскирования PAN-номера карты">
			<type>list</type>
			<enabled>true</enabled>
			<CardPANMaskList>
                <CardPANMask id="Visa Digital"/>
			</CardPANMaskList>
		</param>
        <param name="LastDebitCardBlockOffer" description="Включение экрана с предложением перевода / заказа ЦК при блокировке последней ДК">
			<type>service</type>
			<enabled>true</enabled>
		</param>
        <param name="BlockingNotification" description="Карты с выводом нотификации при блокировке">
			<type>service</type>
          	<enabled>true</enabled>
          	<cardBlockList>    
               <cardBlock id="Visa Digital"/>     
			</cardBlockList>
			<notification>
              <title>Перевести остаток средств перед блокировкой?</title>
              <description>Рекомендуем перед блокировкой карты перевести остаток средств на другую карту или счет. После блокировки карты получить денежные средства можно будет только в офисе банка при предъявлении документа, удостоверяющего личность</description>
              <buttontextcontinue>Продолжить</buttontextcontinue>
              <buttontexttransfer>Перевести</buttontexttransfer>
            </notification>
            <reasonList>
            	<reason id="other"/>
            </reasonList> 
        </param>
        <param name="DebitCardBlockingNotification" description="Дебетовые карты с выводом нотификации при блокировке">
			<type>service</type>
			<enabled>true</enabled>
			<cardBlockList>       
              <cardBlock id="MasterCard Gold"/>
              <cardBlock id="MasterCard Mass"/>
              <cardBlock id="Visa Classic"/>
			</cardBlockList>
			<notification>
				<title>Перевести остаток средств перед блокировкой?</title>
				<description>Рекомендуем перед блокировкой карты перевести остаток средств на другую карту или счет. После блокировки карты получить денежные средства можно будет только в офисе банка при предъявлении документа, удостоверяющего личность</description>
				<buttontextcontinue>Продолжить</buttontextcontinue>
				<buttontexttransfer>Перевести</buttontexttransfer>
			</notification>          	
		</param>
      	<param name="SetPinForCard" description="Установка/смена ПИН-кода карты">
			<enabled>true</enabled>
			<warningEnabled>true</warningEnabled>
			<showTutorial>false</showTutorial>
			<demoEnabled>true</demoEnabled>
			<texts>
				<text id="4" value="После установки не забудьте активировать новый ПИН-код в банкомате Сбербанка. Для активации вставьте карту в банкомат, введите новый ПИН-код и запросите баланс."></text>
			</texts>
		</param>
        <param name="SetPayrollCard" description="Прикрепление карты к зарплатному договору">
     		<enabled>true</enabled>
        </param>
        <param name="SetPayrollCardStage2" description="Прикрепление карты к зарплатному договору (версия 2)">
     	 <enabled>true</enabled>
         <OfferLink>http://www.sberbank.ru/common/img/uploaded/files/pdf/policy.pdf</OfferLink>
      </param> 
        <param name="PayrollCardDeeplinkEnabled" description="Переход по диплинку к зарплатному договору">
     		<enabled>true</enabled> 		   
    	</param>
		<param name="pin_number" description="">
			<type>setting</type>
			<enabled>true</enabled>
			<number>320</number>
		</param>
		<param name="alf" description="">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="uak" description="">
			<type>setting</type>
			<enabled>true</enabled>
			<syncContacts>true</syncContacts>
		</param>
		<param name="avatar" description="">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="rating" description="">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="standin" description="">
			<type>setting</type>
			<enabled>true</enabled>
			<host>node0.online.sberbank.ru</host>
		</param>
		<param name="gamification" description="">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="itunes_cards" description="">
			<type>service</type>
			<enabled>true</enabled>
		</param>
		<param name="aeroexpress" description="">
			<type>service</type>
			<enabled>true</enabled>
		</param>
      	<param name="statement" description="Выписка по истории операций">
            <type>list</type>
            <enabled>true</enabled>
            <nodes>
                <node id="node0.online.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                    <StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>120</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="node1.online.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>120</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="node2.online.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>120</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="node3.online.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>120</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="greenfield1.online.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>180</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="mobile.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>150</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>2</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>180</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>180</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                    <cardStatementOperations>true</cardStatementOperations>
                  	<StatementOperationsLimit>1000</StatementOperationsLimit>
                    <cardStatementTutorial>true</cardStatementTutorial>
                  	<statementCalendarLimit>180</statementCalendarLimit>
                  	<statementCalendarLimitInfo>true</statementCalendarLimitInfo>
                  	<statementPagination>true</statementPagination>
                  	<statementPaginationSize>200</statementPaginationSize>
                  	<statementPaginationLimit>30</statementPaginationLimit>
                </node>
            </nodes>
        </param>
		<param name="VMT" description="VISA MoneyTransfer">
			<type>limit</type>
			<enabled>true</enabled>
			<minamount>1</minamount>
			<maxamount>30000</maxamount>
			<cumulative>30000</cumulative>
			<currency>RUB</currency>
		</param>
		<param name="MCMS" description="MasterCard MoneySend">
			<type>limit</type>
			<enabled>true</enabled>
			<minamount>1</minamount>
			<maxamount>30000</maxamount>
			<cumulative>150000</cumulative>
			<currency>RUB</currency>
		</param>
		<param name="persInformation" description="Personal information">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="moneybox" description="">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="RurPaymentAddressInnExclude" description="Исключение Адреса и ИНН из перевода Клиенту">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="tarifPlanParams" description="">
			<type>list</type>
			<enabled>true</enabled>
			<tarifPlans>
				<tarifPlan id="0">
					<phoneNumbers>
						<phoneNumber cntr="ru" prior="1" addInfo="По России бесплатно (МТС, Билайн, Мегафон, Tele2, Yota, Мотив)" pin="320">900</phoneNumber>
						<phoneNumber cntr="other" prior="2" addInfo="Из-за границы по тарифу оператора" pin="320">+7(495) 500-55-50</phoneNumber>
					</phoneNumbers>
				</tarifPlan>
				<tarifPlan id="1">
					<phoneNumbers>
						<phoneNumber cntr="ru" prior="1" addInfo="По России бесплатно" pin="0">8-800-555-02-55</phoneNumber>
						<phoneNumber cntr="other" prior="2" addInfo="Из-за границы по тарифу оператора" pin="0">+7(495) 669-06-38</phoneNumber>
					</phoneNumbers>
				</tarifPlan>
				<tarifPlan id="2">
					<phoneNumbers>
						<phoneNumber cntr="ru" prior="1" addInfo="По России бесплатно (МТС, Билайн, Мегафон, Tele2, Yota, Мотив)" pin="320">900</phoneNumber>
						<phoneNumber cntr="other" prior="2" addInfo="Из-за границы по тарифу оператора" pin="320">+7(495) 500-55-50</phoneNumber>
					</phoneNumbers>
				</tarifPlan>
				<tarifPlan id="3">
					<phoneNumbers>
						<phoneNumber cntr="ru" prior="1" addInfo="По России бесплатно" pin="0">8-800-333-22-33</phoneNumber>
						<phoneNumber cntr="other" prior="2" addInfo="Из-за границы по тарифу оператора" pin="0">+7(495) 544-45-40</phoneNumber>
					</phoneNumbers>
				</tarifPlan>
			</tarifPlans>
		</param>
		<param name="HiddenStrings" description="Скрываемые сообщения">
			<type>strings</type>
			<strings>
				<string>Регион сохранен</string>
				<string>Обратите внимание: последний раз Вы совершали данный платеж</string>
				<string>Обратите внимание! Не совпадает ФИО получателя.</string>
				<string>вы можете выполнить операцию без подтверждения в контактном центре</string>
				<string>Операция превысила суточный лимит.</string>
				<string>За выполнение данной операции комиссия не взимается</string>
				<string>Обратите внимание! Вы можете выполнить операцию без подтверждения</string>
				<string>Не удается получить карту перевода по указанному номеру телефона</string>
				<string>Счет списания и счет зачисления должны быть различны</string>
				<string>Операцию возможно выполнить только на вклад открытый в</string>
				<string>Ваш платеж успешно отправлен в банк на обработку!</string>
				<string>Операция успешно исполнена. Спасибо, что Вы воспользовались «Сбербанк Онлайн»!</string>
				<string>Ваша заявка успешно отправлена в банк! Спасибо, что воспользовались системой "Сбербанк ОнЛайн"!</string>
				<string>АБС не доступна. Получение информации не возможно.</string>
				<string>Информация из АБС временно недоступна.</string>
				<string>По некоторым Вашим картам информация недоступна.</string>
				<string>За выполнение данной операции комиссия не взимается.</string>
				<string>За данную операцию может взиматься комиссия в соответствии с тарифами банка. Сумму комиссии Вы можете посмотреть на сайте банка.</string>
				<string>В данный момент внешняя система неактивна.</string>
				<string>Неверная авторизация. Неактивный mGUID.</string>
				<string>Ваша заявка успешно отправлена в банк! После исполнения заявки Вы увидите созданный автоплатеж, выбрав пункт «Управление автоплатежами» в разделе «Мои автоплатежи» личного меню. Спасибо, что воспользовались системой «Сбербанк Онлайн»!</string>
				<string>за данную операцию может взиматься комиссия</string>
				<string>Значение данного поля изменилось. При необходимости Вы можете его отредактировать</string>
				<string>Платеж успешно отправлен в банк. Спасибо, что воспользовались «Сбербанк Онлайн»!</string>
				<string>Обратите внимание! Вы не можете совершить операцию на сумму больше</string>
				<string>Обратите внимание! Доступный лимит для совершения операции составляет</string>
				<string>Доступ к операции запрещен!</string>
				<string>Изменение данных невозможно в данный момент</string>
              	<string>вы превысили суточный лимит денежных средств по операциям</string>
              	<string>Обратите внимание! Вы установили лимит на ежедневные</string>
              	<string>ru.sbrf.sbol.erib.modules.exceptions.IllegalTokenCreationStateException: Не заполнен ERIBAuthInfoContext</string>
			</strings>
		</param>
		<param name="ReplaceableStrings" description="Заменяемые сообщения">
			<type>strings</type>
			<strings>
				<string>
					<old>Операция превышает суточный лимит. Вы можете уменьшить сумму или для исполнения операции Вам потребуется подтвердить ее через Контактный центр банка.</old>
					<new>Вы превысили лимит по текущей операции. Данный лимит действует в течение 24 часов. Вы можете уменьшить сумму или для исполнения операции Вам потребуется подтвердить ее через Контактный центр банка.</new>
				</string>
				<string>
					<old>При выполнении этой операции Вы превысите суточный лимит для совершения переводов и оплаты услуг. Данная операция будет исполнена банком только после того, как Вы подтвердите ее через Контактный центр банка по телефонам +7 (495) 500 5550, 8 (800) 555 5550.</old>
					<new>При выполнении этой операции вы превысите лимит на совершение переводов и оплаты услуг. Данный лимит действует в течение 24 часов. Вы можете уменьшить сумму или для исполнения операции Вам потребуется подтвердить ее через Контактный центр банка.</new>
				</string>
				<string>
					<old>Вы превысили лимит по количеству операций перевода средств, выполняемых в течение суток. Операцию необходимо подтвердить в Контактном центре банка, позвонив по телефонам 8 (800) 555 5550, +7 (495) 500 5550.</old>
					<new>Вы превысили лимит по количеству переводов, выполняемых в течение 24 часов. Операцию необходимо подтвердить в Контактном центре банка, позвонив по телефонам 8 (800) 555 5550, +7 (495) 500 5550.</new>
				</string>
				<string>
					<old>Вы превысили лимит по количеству операций перевода средств, выполняемых в течение суток. Пожалуйста, повторите операцию позже.</old>
					<new>Вы превысили лимит по количеству переводов, выполняемых в течение 24 часов. Пожалуйста, повторите операцию позже.</new>
				</string>
				<string>
					<old>Вы превысили лимит на сумму операций перевода средств, выполняемых в течение суток. Операцию необходимо подтвердить в Контактном центре банка, позвонив по телефонам 8 (800) 555 5550, +7 (495) 500 5550.</old>
					<new>Вы превысили лимит на сумму операций перевода средств, выполняемых в течение 24 часов. Операцию необходимо подтвердить в Контактном центре банка, позвонив по телефонам 8 (800) 555 5550, +7 (495) 500 5550.</new>
				</string>
              	<string>
					<old>
                    Вы превысили суточный лимит денежных средств по операциям. Пожалуйста повторите попытку позже.
                    </old>
                    <new>
                    Вы превысили лимит по сумме переведенных средств. Данный лимит действует в течение 24 часов. Пожалуйста повторите попытку позже.
                    </new>
                </string>
				<string>
					<old>Вы превысили лимит на сумму перевода средств, выполняемых в течение суток.</old>
					<new>Вы превысили лимит на сумму перевода средств. Данный лимит действует в течение 24 часов.</new>
				</string>
				<string>
					<old>Регистрация перевода не возможна, у вас уже имеются зарегистрированные не выплаченные переводы</old>
					<new>Чтобы сделать новый заказ, снимите деньги по активному коду в банкомате или отмените заказ в истории операций. Также, можно сделать заказ по другой карте.</new>
				</string>
				<string>
					<old>Ваш логин заблокирован. Повторите попытку позже.</old>
					<new>Вход в Сбербанк Онлайн заблокирован. Если вы забыли пароль, смените пользователя для повторной регистрации.</new>
				</string>
              	<string>
					<old>Неверный логин или пароль!</old>
					<new>Вы ввели неверный пароль. У вас осталось 2 попытки. Если вы забыли пароль, смените пользователя для повторной регистрации.</new>
				</string>
              	<string>
					<old>Неверный логин или пароль. Следующая неверная попытка заблокирует вход в Сбербанк Онлайн на 02 мин</old>
					<new>Вы ввели неверный пароль. Следующая неверная попытка заблокирует вход на 02 мин. Если вы забыли пароль, смените пользователя для повторной регистрации.</new>
				</string>
                <string>
					<old>Вы ввели неправильный идентификатор или пароль из SMS. Пожалуйста, попробуйте снова.</old>
					<new>Вы ввели неправильный идентификатор или код из СМС. Пожалуйста, попробуйте снова.</new>
				</string>
              	<string>
					<old>Вы превысили количество попыток ввода пароля для подтверждения операции. Пожалуйста, создайте новую заявку на регистрацию приложения.</old>
					<new>Вы превысили количество попыток ввода кода для подтверждения операции. Пожалуйста, создайте новую заявку на регистрацию приложения.</new>
				</string>
			</strings>
		</param>
		<param name="Manual" description="Руководство пользователя">
			<type>link</type>
			<link>http://sberbank.ru/common/img/uploaded/files/pdf/Rukovodstvo_polzovatelya_iPhone.pdf</link>
		</param>
		<param name="hide_category" description="">
			<type>list</type>
			<enabled>true</enabled>
			<categories block="mobile.sberbank.ru">
				<category>958</category>
				<category>960</category>
              	<category>277</category>
			</categories>
          	<categories block="node0">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
			<categories block="node1">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
			<categories block="node2">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
			<categories block="node3">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
          	<categories block="node4">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
			<categories block="greenfield1">
              	<category>958</category>
				<category>960</category>
				<category>964</category>
				<category>277</category>
			</categories>
			<categories block="greenfield2">
              	<category>958</category>
				<category>960</category>
				<category>964</category>
				<category>277</category>
			</categories>
          	<categories block="ift-node1-mp.testonline.sberbank.ru">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
            <categories block="ift-node0-mp.testonline.sberbank.ru">
              	<category>277</category>
			</categories>
          	<categories block="ift-node2-mp.testonline.sberbank.ru">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
            <categories block="ift-node3-mp.testonline.sberbank.ru">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
            <categories block="ift-node4-mp.testonline.sberbank.ru">
                <category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
          	<categories block="ift-node5-mp.testonline.sberbank.ru">
              	<category>958</category>
				<category>960</category>
				<category>277</category>
			</categories>
		</param>
		<param name="craudgifting" description="switch for craudgifting">
			<type>setting</type>
			<languages localeId="ru" enabled="true"/>
			<languages localeId="en" enabled="false"/>
			<receivers>15</receivers>
		</param>
		<param name="hide_receiver" description="Скрываемые ПУ по расч.счету">
			<type>list</type>
			<receiver>
				<receiverAccount>40703810838000001730</receiverAccount>
				<receiverAccount>40703810000020105994</receiverAccount>
				<receiverAccount>40703810340350104626</receiverAccount>
				<receiverAccount>40703810400020008374</receiverAccount>
				<receiverAccount>40703810838060051270</receiverAccount>
				<receiverAccount>40703810501200000086</receiverAccount>
				<receiverAccount>40703810338040005076</receiverAccount>
				<receiverAccount>40703810300001400860</receiverAccount>
				<receiverAccount>40703810700001449489</receiverAccount>
				<receiverAccount>40703810697950000000</receiverAccount>
				<receiverAccount>40703810838090000738</receiverAccount>
				<receiverAccount>40703810287810000000</receiverAccount>
				<receiverAccount>40703810238000000975</receiverAccount>
				<receiverAccount>40703810300000000065</receiverAccount>
				<receiverAccount>40703810300020106444</receiverAccount>
				<receiverAccount>30233810800002100002</receiverAccount>
				<receiverAccount>40703810400020008390</receiverAccount>
				<receiverAccount>40702810700020001166</receiverAccount>
				<receiverAccount>40703810300020000003</receiverAccount>
				<receiverAccount>40703810638260001712</receiverAccount>
				<receiverAccount>40703810538000003135</receiverAccount>
				<receiverAccount>40703810038000002584</receiverAccount>
				<receiverAccount>40703810238000002575</receiverAccount>
				<receiverAccount>40703810838040005110</receiverAccount>
				<receiverAccount>40703810038120028888</receiverAccount>
				<receiverAccount>40703810742050001889</receiverAccount>
				<receiverAccount>40703810700000000261</receiverAccount>
				<receiverAccount>40703810938060146056</receiverAccount>
				<receiverAccount>40703810842000000028</receiverAccount>
				<receiverAccount>40703810649770000700</receiverAccount>
				<receiverAccount>40703810038060102864</receiverAccount>
				<receiverAccount>40703810940020100046</receiverAccount>
				<receiverAccount>40703810938040005463</receiverAccount>
				<receiverAccount>40703810038040100912</receiverAccount>
				<receiverAccount>40703810038290071192</receiverAccount>
				<receiverAccount>40703810555040000121</receiverAccount>
				<receiverAccount>40703810623000008598</receiverAccount>
				<receiverAccount>40703810955090106280</receiverAccount>
				<receiverAccount>40703810238110001411</receiverAccount>
				<receiverAccount>40703810438180133973</receiverAccount>
				<receiverAccount>40703810738110100676</receiverAccount>
				<receiverAccount>40703810400000004744</receiverAccount>
				<receiverAccount>40703810000000000072</receiverAccount>
				<receiverAccount>40703810838110100628</receiverAccount>
				<receiverAccount>40703810338260101174</receiverAccount>
				<receiverAccount>40703810638040005611</receiverAccount>
				<receiverAccount>40703810938050001321</receiverAccount>
				<receiverAccount>40703810755100000010</receiverAccount>
				<receiverAccount>40703810138170002547</receiverAccount>
				<receiverAccount>40703810575000000009</receiverAccount>
				<receiverAccount>40703810000000001150</receiverAccount>
				<receiverAccount>40703810838000070062</receiverAccount>
				<receiverAccount>40703810238000001301</receiverAccount>
				<receiverAccount>40703810955040099198</receiverAccount>
				<receiverAccount>40703810338320100413</receiverAccount>
				<receiverAccount>40703810654400000542</receiverAccount>
				<receiverAccount>40703810238290100685</receiverAccount>
				<receiverAccount>40703810925000103890</receiverAccount>
				<receiverAccount>40703810438000001266</receiverAccount>
				<receiverAccount>40703810738000003116</receiverAccount>
				<receiverAccount>40703810738260100759</receiverAccount>
				<receiverAccount>40703810738170101233</receiverAccount>
				<receiverAccount>40703810300030000036</receiverAccount>
				<receiverAccount>40703810654060100293</receiverAccount>
				<receiverAccount>40703810138000001155</receiverAccount>
				<receiverAccount>40703810451150100097</receiverAccount>
				<receiverAccount>40703810338110001751</receiverAccount>
				<receiverAccount>40703810338000000891</receiverAccount>
				<receiverAccount>40703810538070101258</receiverAccount>
				<receiverAccount>40703810038260001820</receiverAccount>
				<receiverAccount>40703810038170100772</receiverAccount>
				<receiverAccount>40703810806000000112</receiverAccount>
				<receiverAccount>40703810262000000624</receiverAccount>
				<receiverAccount>40703810438180000307</receiverAccount>
				<receiverAccount>40703810260300000879</receiverAccount>
				<receiverAccount>40703810200000011387</receiverAccount>
				<receiverAccount>40703810300020000003</receiverAccount>
              	<receiverAccount>40703810238000004230</receiverAccount>
			</receiver>
		</param>
      	<param name="showCorporateCard" description="Глобальный рубильник показа корпортаивных карт">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="charity_text" description="Текст при попытке оплаты благотворительного ПУ">
			<type>strings</type>
			<strings>
				<string localeId="ru">"К сожалению, оплата в пользу благотворительных организаций не может осуществляться в мобильном приложении для iOS по независящим от нас причинам.
Вы можете совершить оплату через веб-версию Сбербанк Онлайн, любое отделение или банкомат Сбербанка."</string>
			</strings>
		</param>
		<param name="self_registration_translate" description="Замена строк при саморегистрации если локализация отлична от дефолтной">
			<type>strings</type>
			<strings>
				<string>
					<RU>попытки</RU>
					<EN>attempts</EN>
				</string>
				<string>
					<RU>Пароль не должен повторять старые пароли за последние 3 месяца</RU>
					<EN>The password must not repeat the old passwords in the last 3 months</EN>
				</string>
				<string>
					<RU>Введенный идентификатор уже используется в системе. Введите другое значение</RU>
					<EN>The entered ID is already in use in the system. Enter a different value</EN>
				</string>
			</strings>
		</param>
		<param name="fundInfo" description="Получение информации о наличии у контактов МП про-версии">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="wrongpass" description="">
			<type>list</type>
			<enabled>true</enabled>
			<attempts>
				<attempt>
					<localeId>ru</localeId>
					<count>1</count>
					<string>Вы неверно ввели код 1 раз. Если вы 3 раза введете код неверно, вы будете заблокированы на 1 час</string>
				</attempt>
				<attempt>
					<localeId>ru</localeId>
					<count>2</count>
					<string>Вы неверно ввели код 2 раза. У вас осталась 1 попытка. Если вы забыли код на вход, воспользуйтесь функцией «забыл код на вход».</string>
				</attempt>
			</attempts>
		</param>
		<param name="marketplaceMainScreenOffer" description="">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="SupportMainEntryPointEnabled" description="Доступность точки входа в чат Сбербанка на Главной">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="newmarketplace" description="Витрина 7.3.1">
			<type>setting</type>
			<enabled>true</enabled>
          	<recommendedEnabled>false</recommendedEnabled>
            <marketplaceBackendCMSTimeOut>100000</marketplaceBackendCMSTimeOut>
          	<marketplaceBackendStandaloneJson>https://test.stat.online.sberbank.ru/SUPERAPP/sbolconfig/ios.catalog.json</marketplaceBackendStandaloneJson>
			<urls>
				<url name="marketplace_v1" url="http://sbertech.online/marketplace/config.ios.8.15.xml" version="9.1.0"/>
				<url name="marketplace_v2" url="http://sbertech.online/marketplace/config.ios.9.2.xml" version="9.2.0"/>
				<url name="marketplace_v2" url="https://stories-stat.online.sberbank.ru/MEDIA/marketplace/config.ios.9.3.xml" version="9.3.0"/>
				<url name="marketplace_v2" url="https://test.stat.online.sberbank.ru/SUPERAPP/sbolconfig/config.ios.9.8.xml" version="9.8.0"/>
              	<url name="marketplace_v2" url="https://test.stat.online.sberbank.ru/SUPERAPP/sbolconfig/config.ios.10.1.xml" version="10.1.0"/>
			</urls>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                    <marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                 	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                    <marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                    <marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="node4.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
              <node id="node5.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="194.186.207.23">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>false</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                 	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>              
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>  
              	<node id="ift-node6-mp.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node> 
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>  
				<node id="psinode2.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
				<node id="psinode1.testonline.sberbank.ru">
					<enabled_Marketplace_2_0>true</enabled_Marketplace_2_0>
					<mainEntryEnabled>true</mainEntryEnabled>
                  	<personalizationEnabled>true</personalizationEnabled>
                  	<marketplaceBackendEnabled>true</marketplaceBackendEnabled>
				</node>
			</nodes>
		</param>
		<param name="marketplace_search_ignore" description="Не отображение в поиске определенных поставщиков услуг">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="tokenizationBINs" description="">
          <type>list</type>
          <enabled>true</enabled>
          <BINs paymentSystem="MasterCard">
            <BINrange start="522860"/>
            <BINrange start="531310"/>
            <BINrange start="533205"/>
            <BINrange start="533208"/>
            <BINrange start="536961"/>
            <BINrange start="533669"/>
            <BINrange start="545152"/>
            <BINrange start="546901"/>
            <BINrange start="546902" end="546913"/>
            <BINrange start="546916" end="546918"/>
            <BINrange start="546920"/>
            <BINrange start="546922"/>
            <BINrange start="546925" end="546933"/>
            <BINrange start="546935"/>
            <BINrange start="546937" end="546956"/>
            <BINrange start="546959" end="546964"/>
            <BINrange start="546966" end="546970"/>
            <BINrange start="546972"/>
            <BINrange start="546974" end="546977"/>
            <BINrange start="546998" end="546999"/>
            <BINrange start="547927"/>
            <BINrange start="548401"/>
            <BINrange start="548402" end="548403"/>
            <BINrange start="548405" end="548407"/>
            <BINrange start="548410" end="548413"/>
            <BINrange start="548416"/>
            <BINrange start="548420"/>
            <BINrange start="548422"/>
            <BINrange start="548425" end="548428"/>
            <BINrange start="548430" end="548432"/>
            <BINrange start="548435" end="548436"/>
            <BINrange start="548438"/>
            <BINrange start="548440"/>
            <BINrange start="548442" end="548445"/>
            <BINrange start="548447" end="548452"/>
            <BINrange start="548454" end="548456"/>
            <BINrange start="548459" end="548464"/>
            <BINrange start="548466"/>
            <BINrange start="548468" end="548469"/>
            <BINrange start="548470"/>
            <BINrange start="548472"/>
            <BINrange start="548476" end="548477"/>
            <BINrange start="548498" end="548499"/>
            <BINrange start="557000"/>
		  </BINs>
		  <BINs paymentSystem="VISA">
            <BINrange start="417398"/>
            <BINrange start="427417"/>
            <BINrange start="427427"/>
            <BINrange start="427432"/>
            <BINrange start="427448"/>
            <BINrange start="427601" end="427613"/>
            <BINrange start="427616" end="427618"/>
            <BINrange start="427620"/>
            <BINrange start="427622"/>
            <BINrange start="427625" end="427633"/>
            <BINrange start="427635" end="427646"/>
            <BINrange start="427648" end="427656"/>
            <BINrange start="427659" end="427664"/>
            <BINrange start="427666" end="427670"/>
            <BINrange start="427672"/>
            <BINrange start="427674" end="427677"/>
            <BINrange start="427680" end="427687"/>
            <BINrange start="427689"/>
            <BINrange start="427699"/>
            <BINrange start="427901" end="427913"/>
            <BINrange start="427916" end="427918"/>
            <BINrange start="427920"/>
            <BINrange start="427922"/>
            <BINrange start="427925" end="427933"/>
            <BINrange start="427935" end="427946"/>
            <BINrange start="427948" end="427956"/>
            <BINrange start="427959" end="427964"/>
            <BINrange start="427966" end="427970"/>
            <BINrange start="427972"/>
            <BINrange start="427974" end="427975"/>
            <BINrange start="427977"/>
            <BINrange start="427999"/>
            <BINrange start="481776"/>
            <BINrange start="481779"/>
            <BINrange start="481781"/>
            <BINrange start="483983"/>
            <BINrange start="485463"/>
		</BINs>
		</param>
		<param name="mastercard_tokenisation" description="">
          <type>setting</type>
          <enabled>true</enabled>
      </param>
      <param name="visa_tokenisation" description="">
        <type>setting</type>
        <enabled>true</enabled>
      </param>
      <param name="visa_tokenization_new" description="">
        <type>setting</type>
        <enabled>true</enabled>
		</param>
        <param name="nfcTokensManagementMain" description="Управление жизненным циклом токенов">
        	<type>list</type>
      		<enabled>true</enabled>
            <nfcTokensManagementVisa>true</nfcTokensManagementVisa>
            <nfcTokensManagementMC>true</nfcTokensManagementMC>
            <nfcTokensManagementTabs>false</nfcTokensManagementTabs>
			<nodes>
                <node id="greenfield1.online.sberbank.ru">
                    <tabs>true</tabs>
                </node>
                <node id="node5.online.sberbank.ru">
                    <tabs>true</tabs>
                </node>
            </nodes>
        </param>
      	<param name="statementWithLogo" description="Красивая выписка">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="birthday" description="">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="hidealfoperations" description="Скрываем операции АЛФ">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="aim_status" description="Индикация выполнения цели">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
        <param name="MessengerPermissions" description="">
                        <type>list</type>
			<authMessenger>true</authMessenger>
          <MessengerNewYearPostcardURL>https://test.stat.online.sberbank.ru/Dialogues/SberkotNewYear.mp4</MessengerNewYearPostcardURL>
          <MessengerNewYearPostcardText>Новый год — время чудес! Делитесь счастьем!</MessengerNewYearPostcardText>
          <MessengerGiftsDefaultPostcardId>giftpostcard</MessengerGiftsDefaultPostcardId>
          <MessengerGiftsDefaultPostcardExtension>mp4</MessengerGiftsDefaultPostcardExtension>
          <MessengerShareBaseLinkUrl>https://www.sberbank.ru/dl/jc/psi/index.html?channel=</MessengerShareBaseLinkUrl>
			<nodes>
				<node id="node0.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                    <MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>false</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                  	<MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                  	<MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
				<node id="node1.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                    <MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                  	<DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
				<node id="node2.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                 	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                  	<DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
				<node id="node3.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2> 
                    <ChatBotForward>false</ChatBotForward>
                  	<DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              	<node id="node4.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                  	<DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>false</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                  	<DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats> 
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
				<node id="greenfield2.online.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                  	<DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
            	<node id="ift-node1-mp.testonline.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute> 
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                    <MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute> 
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                    <MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                  	<ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              <node id="ift-node5-mp.testonline.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                  	<ChatBotAttachFromCameraEnabled>false</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                  <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>false</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                  	<ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              	<node id="mobile.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>true</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>false</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget> 
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              <node id="mobile4.sberbank.ru">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>true</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>true</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              	<node id="mobile.sberbank.ru:4459">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial> 
                    <MessengerP2PRetranslation>true</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>false</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>true</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>true</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
              	<node id="mobile.sberbank.ru:4460">
                 	<MessengerLoginNew>true</MessengerLoginNew>
                  	<MessengerBlockContactWithReason>true</MessengerBlockContactWithReason>
                 	<timeToRefreshUnread>600</timeToRefreshUnread>
                    <MessengerLinks>true</MessengerLinks>
                  	<MessengerMarkdownLinks>true</MessengerMarkdownLinks>
                    <MessengerPostcardFirework>true</MessengerPostcardFirework>
                    <MessengerPostcardSend>true</MessengerPostcardSend>
                  	<MessengerPostcardForNonClient>true</MessengerPostcardForNonClient>
                  	<MessengerPostcardUGCVideo>true</MessengerPostcardUGCVideo>
                    <MessengerVoicePostcardNew>true</MessengerVoicePostcardNew>
                    <MessengerVoicePostcardTutorial>true</MessengerVoicePostcardTutorial>
                    <MessengerP2PRetranslation>true</MessengerP2PRetranslation>
                  	<MessengerDocDoc>true</MessengerDocDoc>
                  	<MessengerOpenDialogWithDeepLink>true</MessengerOpenDialogWithDeepLink>
                    <MessengerPin>true</MessengerPin>
                    <MessengerTyping>true</MessengerTyping>
                    <MessengerChatMute>true</MessengerChatMute>
                    <MessengerForward>true</MessengerForward>
                    <MessengerGroupChatEnabled>true</MessengerGroupChatEnabled>
                    <MessengerGroupChat>false</MessengerGroupChat>
                    <MessengerGroupChatAvatarLoadingEnabled>true</MessengerGroupChatAvatarLoadingEnabled>
                    <ChatWithBankLikeGroupchat>true</ChatWithBankLikeGroupchat>
                    <ChatWithBankNewYearEnabled>true</ChatWithBankNewYearEnabled>
                    <MessengerSaveContact>true</MessengerSaveContact>
                    <DraftMessagesEnabled>false</DraftMessagesEnabled>
                    <DraftMessage900Enabled>true</DraftMessage900Enabled>
                    <AttachmentsForChatBotEnabled>true</AttachmentsForChatBotEnabled>
                  	<MessengerChannelsEnabled>true</MessengerChannelsEnabled>
                  	<MessengerChannels_actual>true</MessengerChannels_actual>
                    <MessengerCrowdFunding>true</MessengerCrowdFunding>
                    <MessengerCrowdFundingV2>true</MessengerCrowdFundingV2>
                    <ChatBotForward>false</ChatBotForward>
                    <DownloadingBotAvatarsEnabled>true</DownloadingBotAvatarsEnabled>
                    <MessengerReply>true</MessengerReply>
                    <ChatBotReply>false</ChatBotReply>
                    <MessengerDeleteMessage>true</MessengerDeleteMessage>
                    <MessengerWithoutMoneyPostcard>true</MessengerWithoutMoneyPostcard>
                    <ChatBotAttachFromCameraEnabled>true</ChatBotAttachFromCameraEnabled>
                    <MessengerPaymentSuggestion>true</MessengerPaymentSuggestion>
                    <MessengerPhoto>true</MessengerPhoto>
                    <MessengerPhotoView>true</MessengerPhotoView>
                    <MessengerMoneyButton>true</MessengerMoneyButton>
                    <MessengerP2PWidget>true</MessengerP2PWidget>
                  	<SendOpenDialogEnabled>true</SendOpenDialogEnabled>
                    <MessengerBusinessChats>true</MessengerBusinessChats>
                    <MessengerCrowdfundingListFilter>true</MessengerCrowdfundingListFilter>
                  	<UpdateEribProfileEnabled>true</UpdateEribProfileEnabled>
				</node>
			</nodes>
                </param>
		<param name="AccountClosing" description="Закрытие вкладов 8.0">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
        <param name="local_tips" description="">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="pfmHosts" description="Список хостов для phizPFM">
			<type>list</type>
			<enabled>true</enabled>
			<hosts>
				<host id="node0.online.sberbank.ru">
					<value>pfm.node0.online.sberbank.ru:4433</value>
				</host>
				<host id="node1.online.sberbank.ru">
					<value>pfm.node1.online.sberbank.ru:4433</value>
				</host>
				<host id="node2.online.sberbank.ru">
					<value>pfm.node2.online.sberbank.ru:4433</value>
				</host>
				<host id="node3.online.sberbank.ru">
					<value>pfm.node3.online.sberbank.ru:4433</value>
				</host>
                <host id="node4.online.sberbank.ru">
					<value>node4.online.sberbank.ru:6655</value>
				</host>
				<host id="greenfield1.online.sberbank.ru">
					<value>greenfield1.online.sberbank.ru:6655</value>
				</host>
				<host id="greenfield2.online.sberbank.ru">
					<value>greenfield2.online.sberbank.ru:6655</value>
				</host>
				<host id="194.186.207.23">
					<value>194.186.207.23</value>
				</host>
                <host id="mobile.sberbank.ru">
					<value>194.186.207.23</value>
				</host>
				<host id="ift-node1.testonline.sberbank.ru">
					<value>pfm.ift-node1.testonline.sberbank.ru:4464</value>
				</host>
				<host id="ift-node1-mp.testonline.sberbank.ru">
					<value>pfm.ift-node1.testonline.sberbank.ru:4464</value>
				</host>
                <host id="ift-node0-mp.testonline.sberbank.ru">
					<value>pfm.ift-node1.testonline.sberbank.ru:4464</value>
				</host>
			</hosts>
		</param>
		<param name="PFMConfigFlags" description="Блоки работают по логическому ИЛИ">
		<PfmGlobal>
		</PfmGlobal>
		<PfmNodes>
				<node id="node0.online.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
                    <PFMUserParams>false</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                  	<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                  	<pfmApiVersion>1.30</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                 	<SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                  	<NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>false</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>8.15</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                  	<SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                  	<NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          	  <node id="node4.online.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<PFMUserParams>true</PFMUserParams>
                  	<currentPfmApiVersion description="Устаревший параметр">1.30</currentPfmApiVersion>
					<pfmApiVersion>1.40</pfmApiVersion>
					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                 	<pfmDataOnline>true</pfmDataOnline>
                	<NewALFInHistory>true</NewALFInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                	<NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
         		 <node id="node5.online.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<PFMUserParams>true</PFMUserParams>
                  	<currentPfmApiVersion description="Устаревший параметр">1.30</currentPfmApiVersion>
					<pfmApiVersion>1.40</pfmApiVersion>
					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                 	<pfmDataOnline>true</pfmDataOnline>
                	<NewALFInHistory>true</NewALFInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                	<NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
				<node id="greenfield2.online.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                    <pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
				<node id="194.186.207.23">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                  	<pfmApiVersion>1.30</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <NewBudgetEnabled>false</NewBudgetEnabled>
                    <RemoveOldDashboard>true</RemoveOldDashboard>
				</node>
          		<node id="mobile.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.40</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
                    <RemoveOldDashboard>true</RemoveOldDashboard> 
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                 	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>false</NewBudgetEnabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>false</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
					<PFMSimilarSpendings>false</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
				</node>
          		<node id="ift-node4.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                 	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          		<node id="ift-node4-mp.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          		<node id="ift-node7-mp.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          <node id="ift-node2.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                 	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
           		    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          		<node id="ift-node2-mp.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                    <pfmDataOnline>true</pfmDataOnline>
                    <NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                    <NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          <node id="ift-node5.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                 	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                  	<pfmDataOnline>true</pfmDataOnline>
                  	<NewALFInHistory>true</NewALFInHistory>
                  	<SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
            		<NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
          		<node id="ift-node5-mp.testonline.sberbank.ru">
					<PFMSimilarSpendings>true</PFMSimilarSpendings>
					<currentPfmApiVersion description ="Устаревший параметр">1.30</currentPfmApiVersion>
                    <PFMUserParams>true</PFMUserParams>
					<PFMOfferTips>true</PFMOfferTips>
                  	<pfmApiVersion>1.40</pfmApiVersion>
 					<minAppVersionFromPFMApiVersion>9.1</minAppVersionFromPFMApiVersion>
                  	<pfmDataOnline>true</pfmDataOnline>
                  	<NewALFInHistory>true</NewALFInHistory>
                    <SendALFConnectInHistory>true</SendALFConnectInHistory>
                    <ALFNewPieChartEnabled>true</ALFNewPieChartEnabled>
                  	<NewBudgetEnabled>true</NewBudgetEnabled>
				</node>
			</PfmNodes>
	    </param>
        <param name="PFMTipsCloseEmptyQuizCount" description="Вероятность, с которой пользователю будет предложено выбрать причину скрытия совета">
			<type>setting</type>
			<enabled>false</enabled>
			<value>0.25</value>
		</param>
		<param name="PFMDashboardIncomeHide" description="Дашборд, Доходы, скрытие АЛФ операций">
			<type>list</type>
			<enabledNodes>false</enabledNodes>
			<enabledGlobal>true</enabledGlobal>
			<PfmGlobal>
				<dashboard>true</dashboard>
				<income>true</income>
				<hidealfoperations>true</hidealfoperations>
			</PfmGlobal>
		</param>
        <param name="aim_close" description="Закрытие Цели">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		 <param name="VOIPCallOperator" description="Звонок оператору через интернет">
            <type>list</type>
            <enabled>true</enabled>
            <nodes>
                <node id="node0.online.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="node1.online.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="node2.online.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="node3.online.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="greenfield1.online.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="greenfield2.online.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="194.186.207.23">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="mobile.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node4.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node4-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="psinode1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="psinode2.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node5.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
              	<node id="ift-node7.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <enabledPrelogin>true</enabledPrelogin>
                    <enabledPostlogin>true</enabledPostlogin>
                    <isHidingCallScreenEnabled>true</isHidingCallScreenEnabled>
                    <isInCallStatusBarEnabled>true</isInCallStatusBarEnabled>
                    <isVOIPSessionWarmupEnabled>true</isVOIPSessionWarmupEnabled>
                    <isVOIPNMTEnabled>true</isVOIPNMTEnabled>
                    <isChatWithBankCSIEnabled>true</isChatWithBankCSIEnabled>
                    <CSICommentFieldEnabled>true</CSICommentFieldEnabled>
                </node>
            </nodes>
        </param>
		<param name="ChatBot" description="Диалог с контактом Сбербанк (@900)">
			<type>list</type>
            <enabled>true</enabled>
            <nodes>
                <node id="node0.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="node1.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="node2.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="node3.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
              	<node id="node4.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="greenfield1.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="greenfield2.online.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="mobile.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="mobile4.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node4.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node4-mp.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node5.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="ift-node7-mp.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
              	<node id="ift-node7.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="psinode1.testonline.sberbank.ru">
                    <dialog900>false</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
                <node id="psinode2.testonline.sberbank.ru">
                    <dialog900>true</dialog900>
                    <SmartSearchChatWithBankEnabled>true</SmartSearchChatWithBankEnabled>
                </node>
            </nodes>
        </param>
		<param name="900Permissions" description="">
			<type>list</type>
			<pushAlertTimeInterval>86400</pushAlertTimeInterval>
          	<efsMobileBank>true</efsMobileBank>
			<nodes>
              	<node id="ift-node1.testonline.sberbank.ru">
                  	<efsMobileBank>true</efsMobileBank>
                </node>
              	<node id="ift-node2.testonline.sberbank.ru">
                  	<efsMobileBank>true</efsMobileBank>
                </node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
                  	<efsMobileBank>true</efsMobileBank>
                  	<pushAlertEnabled>true</pushAlertEnabled>
                </node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                  	<efsMobileBank>true</efsMobileBank>
                  	<pushAlertEnabled>true</pushAlertEnabled>
                </node>
              	<node id="ift-node2-mp.testonline.sberbank.ru">
                  	<efsMobileBank>true</efsMobileBank>
					<pushAlertEnabled>true</pushAlertEnabled>
                </node>
				<node id="node0.online.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
                  	<efsMobileBank>true</efsMobileBank>
				</node>
				<node id="greenfield2.online.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
				<node id="194.186.207.23">
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
              	<node id="mobile.sberbank.ru">
					<pushAlertEnabled>true</pushAlertEnabled>
                  	<efsMobileBank>true</efsMobileBank>
				</node>
				<node id="ift-node5-mp.testonline.sberbank.ru">
					<efsMobileBank>true</efsMobileBank>
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<efsMobileBank>true</efsMobileBank>
					<pushAlertEnabled>true</pushAlertEnabled>
				</node>
			</nodes>
		</param>
		<param name="CorePermissions" description="">
			<type>list</type>
			<enabled>true</enabled>
        	<dontShowVersion>false</dontShowVersion>
            <selectCityOnMap>false</selectCityOnMap>
			<nodes>
              	<node id="psinode2.testonline.sberbank.ru">
					<SBTelecom>true</SBTelecom>
                    <SBTelecomV2>true</SBTelecomV2>
                    <EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
                    <enableContactMangager>true</enableContactMangager>
                </node>
              	<node id="psinode1.testonline.sberbank.ru">
					<SBTelecom>true</SBTelecom>
                    <SBTelecomV2>true</SBTelecomV2>
                    <enableContactMangager>true</enableContactMangager>
                </node>
				<node id="node0.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                    <SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                    <OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>      
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                  	<showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                  	<AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>false</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
					<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                    <webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                	<FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>false</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>false</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
            		<mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                  	<sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                 	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                  	<balanceFromPushV2>true</balanceFromPushV2>
                  	<PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="ift-node0-mp.online.sberbank.ru">
					<coreQR>false</coreQR>
					<SBTelecom>true</SBTelecom>
                    <SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                    <OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>false</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>              
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
                  	<UFSHost></UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                  	<showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                  	<AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>false</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
					<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                    <webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                	<FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>false</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
            		<mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                 	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                  	<balanceFromPushV2>true</balanceFromPushV2>
                  	<PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="node1.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                    <SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>false</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment> 
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                 	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
           	    	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>false</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                  	<AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                    <historyList_v2>true</historyList_v2>
                 	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>284</billing>
   						<provider>621180</provider>
   						<service>297</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
        			<FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>false</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                 	<InstantAppV2>true</InstantAppV2>
                 	<mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="node2.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                    <SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>false</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>              
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                    <fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>284</billing>
   						<provider>500438244</provider>
   						<service>297</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>false</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                 	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                  	<balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="node3.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>false</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
                 
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
					<showUfsHistoryOperations>false</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>284</billing>
   						<provider>500437522</provider>
   						<service>297</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
                  	<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>false</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                  	<balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="node4.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>false</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
                 
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
					<showUfsHistoryOperations>false</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>284</billing>
   						<provider>500437522</provider>
   						<service>297</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
                  	<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>false</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                  	<balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment> 
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                  	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>284</billing>
   						<provider>550470225</provider>
   						<service>297</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>false</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<googleMapsEnabled>true</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                 	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="greenfield2.online.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>false</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost></UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                  	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>284</billing>
   						<provider>550470225</provider>
   						<service>297</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<SBMProductsViewController>true</SBMProductsViewController>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<googleMapsEnabled>true</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="mobile.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>pfl-psi.efstst.sigma.sbrf.ru:443</UFSHost>
            		<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>4</billing>
   						<provider>3</provider>
   						<service>3</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>false</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                 
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                 	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
              		<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>true</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="ift-node2.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                   	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                  	<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>true</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="ift-node5.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
                  	<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                   	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                  	<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                 	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                 
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                 	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
    				<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled> 
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                  
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                 	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
    				<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="ift-node2-mp.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                  
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                  	<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>true</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                    <PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
					<coreQR>false</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                 
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                  	<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                 
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
                  	<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                    <newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="10.21.152.7">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
                  	<UFSHost>sbt-oafs-498.sigma.sbrf.ru:443</UFSHost>
                 	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
					<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                  	<EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
          			<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>false</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>false</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                    <PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              <node id="ift-c-mp.testonline.sberbank.ru">
					<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>                
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                	<pensionRegistration>true</pensionRegistration>
                	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>ift.testefs.sberbank.ru:443</UFSHost>
                  	<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                 	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                    <importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
    				<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                	<newProductsVC>true</newProductsVC>
                	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                  <refactoredServiceEnabled>true</refactoredServiceEnabled>
                    <googleMapsEnabled>false</googleMapsEnabled>
                	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                	<authBlockingScreen>true</authBlockingScreen>
                	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
				</node>
              	<node id="mobile4.sberbank.ru">
                  	<coreQR>true</coreQR>
					<SBTelecom>true</SBTelecom>
                  	<SBTelecomV2>true</SBTelecomV2>
					<CreditRating>false</CreditRating>
					<CreditRating_v2>false</CreditRating_v2>
                  	<OKBRating>true</OKBRating>
					<EnableBetaVersion>
						<version>8.1.2</version>
						<version>8.1.1</version>
					</EnableBetaVersion>
					<enableArrests>true</enableArrests>
					<cardDelivery>true</cardDelivery>
					<loanTable>true</loanTable>
					<hideRegion>true</hideRegion>
					<pciDss>true</pciDss>
                  	<cashByCode>true</cashByCode>
					<creditCardAutorepayment>true</creditCardAutorepayment>
					<governmentServices>true</governmentServices>
					<pensionTransfer>true</pensionTransfer>
					<pensionCertificate>true</pensionCertificate>
                  	<governmentServices_actual>true</governmentServices_actual>
					<pensionTransfer_actual>true</pensionTransfer_actual>
					<pensionCertificate_actual>true</pensionCertificate_actual>
                  	<pensionRegistration>true</pensionRegistration>
                  	<governmentAnimationSearching>true</governmentAnimationSearching>
					<blockedCardsStatusWay4>true</blockedCardsStatusWay4>
					<autoTransfer>true</autoTransfer>
					<autoTransferMinAmountEnabled>true</autoTransferMinAmountEnabled>
					<autoTransferMinAmount>30</autoTransferMinAmount>
                  	<UFSHost>pfl-psi.efstst.sigma.sbrf.ru:443</UFSHost>
            		<coreCreditCardInfo_v2>true</coreCreditCardInfo_v2>
                    <coreCreditCardInfo_v3>true</coreCreditCardInfo_v3>
                  	<OmniChannelHistory>true</OmniChannelHistory>
                  	<showUfsHistoryOperations>true</showUfsHistoryOperations>
                    <showSpasibo>true</showSpasibo>
                  	<enableContactMangager>true</enableContactMangager>
                    <AuthCyrrilicKeypadEnabled>true</AuthCyrrilicKeypadEnabled>
                  	<showCorporateCard>true</showCorporateCard>
                  	<autoTouchID>true</autoTouchID>
                  	<suggestionsEnabled>true</suggestionsEnabled>
                   	<historyList_v2>true</historyList_v2>
                  	<shimmersEnabled>true</shimmersEnabled>
                  	<skeletonsEnabled>true</skeletonsEnabled>
                  	<early2018EnterAnimation>true</early2018EnterAnimation>
                  	<fastLoginOnMessengerPushEnabled>true</fastLoginOnMessengerPushEnabled>
                  	<currenciesInOperationsVCEnabled>false</currenciesInOperationsVCEnabled>
                    <EribPenaltyDocumentsSavingAllowed>true</EribPenaltyDocumentsSavingAllowed>
                    <EribFinesLoadingAutoretry>true</EribFinesLoadingAutoretry>
            		<EribStatePaymentShortCutsEnabled>true</EribStatePaymentShortCutsEnabled>
                  	<EribAfterPayInfoEnabled>true</EribAfterPayInfoEnabled>
					<EribServicesDeeplinkEnabled>true</EribServicesDeeplinkEnabled>
                  	<EribPenaltyInPaymentProcessEnabled>true</EribPenaltyInPaymentProcessEnabled>
                  	<EribPenaltyDocumentsMigration>true</EribPenaltyDocumentsMigration>
                  	<charity>
   						<enabled>true</enabled>
   						<billing>4</billing>
   						<provider>3</provider>
   						<service>3</service>
   						<text>Здесь можно перевести любую сумму пострадавшим в Кемерове</text>
					</charity>
					<importantInfoEnabled>false</importantInfoEnabled>
					<historyRouterEnabled>true</historyRouterEnabled>
                  	<SBTelecomSectionOnlyForClients>false</SBTelecomSectionOnlyForClients>
					<webAnalyticsEnabled>true</webAnalyticsEnabled>
                  	<newSectionInvestEnable>true</newSectionInvestEnable>
                  	<newProductsVC>true</newProductsVC>
                  	<newProductsVCv2>true</newProductsVCv2>
                  	<hidingSectionEnabled>true</hidingSectionEnabled>
                  	<orderingSectionEnabled>true</orderingSectionEnabled>
					<hidingSectionTutorialEnabled>false</hidingSectionTutorialEnabled>
                  	<arrestInfoService>true</arrestInfoService>
                    <FastLoginApp>false</FastLoginApp>
                	<PrintAutoSubscriptionCheck>true</PrintAutoSubscriptionCheck>
                    <productNavigationBarMod>3</productNavigationBarMod>
                  	<IsFromAddrBook>true</IsFromAddrBook>
                  	<InstantApp>true</InstantApp>
                  	<InstantAppV2>true</InstantAppV2>
                    <mobilePOSEnabled>true</mobilePOSEnabled>
                  	<earlyLoanRepayment>true</earlyLoanRepayment>
                  	<newProductDetailsUIEnabled>true</newProductDetailsUIEnabled>
                    <newProductDetailsContentEnabled>true</newProductDetailsContentEnabled>
                  	<soundsInAppEnabled>true</soundsInAppEnabled>
                    <hapticsInAppEnabled>true</hapticsInAppEnabled>
                    <sectionsCombination>true</sectionsCombination>
                    <hidingProductsInSectionEnabled>true</hidingProductsInSectionEnabled>
                    <sectionOrderResetEnabled>true</sectionOrderResetEnabled>
                    <refactoredServiceEnabled>true</refactoredServiceEnabled>
                  	<PaymentTransactionsPopUpConfirmNumber>true</PaymentTransactionsPopUpConfirmNumber>
                    <googleMapsEnabled>false</googleMapsEnabled>
                  	<messengerFirstLoginEnabled>false</messengerFirstLoginEnabled>
                  	<authBlockingScreen>true</authBlockingScreen>
                  	<PrintAutoSubscriptionTutorialCheck>true</PrintAutoSubscriptionTutorialCheck>
                    <balanceFromPushV2>true</balanceFromPushV2>
                    <PaymentsRequisiteGroupingEnabled>true</PaymentsRequisiteGroupingEnabled>
                    <PaymentsTransitionToRequisites>true</PaymentsTransitionToRequisites>
                    <feedbackMenuItemEnabled>true</feedbackMenuItemEnabled>
                  	<extendedMainHeader>true</extendedMainHeader>
                </node>
			</nodes>
		</param>
       	<param name="NominalAccounts" description="Право работать с номинальными счетами">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="arrestInfoService" description="">
			<type>setting</type>
			<enabled>true</enabled>
          	<bankruptUrl>https://www.sberbank.ru/ru/person/help-center/bankrupt</bankruptUrl>
			<arrestInfoUrl>https://www.sberbank.ru/ru/person/seizure</arrestInfoUrl>
            <phoneFSSP>8 800 250-39-32</phoneFSSP>
            <workingHoursFSSP>по будням 9:00-18:00(МСК)</workingHoursFSSP>
		</param>
      	<param name="arrestInfoService_v2" description="">
			<type>setting</type>
			<enabled>true</enabled>
          	<bankruptUrl>https://www.sberbank.ru/ru/person/help-center/bankrupt</bankruptUrl>
			<arrestInfoUrl>https://www.sberbank.ru/ru/person/seizure</arrestInfoUrl>
            <phoneFSSP>8 800 250-39-32</phoneFSSP>
            <workingHoursFSSP>по будням 9:00-18:00(МСК)</workingHoursFSSP>
		</param>
    	<param name="ufsOperationDetailHistoryAlert" description="">
			<type>strings</type>
			<strings>
				<string localeId="ru">Вы не можете просмотреть данную операцию через мобильное приложение. Для просмотра воспользуйтесь Web версией Сбербанк Онлайн.</string>
			</strings>
		</param>
 		<param name="integrationPlatform" description="">
			<type>list</type>
			<nodes>
        		<node id="node0.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="node1.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="node2.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="node3.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="node4.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="greenfield1.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="greenfield2.online.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="mobile.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="mobile4.sberbank.ru">
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="ift-node0-mp.testonline.sberbank.ru">
            		<serviceSessionForUFS6AndUFS7>false</serviceSessionForUFS6AndUFS7>
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="ift-node1-mp.testonline.sberbank.ru">
            		<serviceSessionForUFS6AndUFS7>false</serviceSessionForUFS6AndUFS7>
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
            		<serviceSessionForUFS6AndUFS7>false</serviceSessionForUFS6AndUFS7>
            		<startSessionUFS7>true</startSessionUFS7>
        		</node>
        		<node id="ift-node5-mp.testonline.sberbank.ru">
            		<serviceSessionForUFS6AndUFS7>false</serviceSessionForUFS6AndUFS7>
            		<startSessionUFS7>true</startSessionUFS7>
           			<pathUFSToMigrate>/sm-uko/v2/session/create</pathUFSToMigrate>
        		</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
            		<serviceSessionForUFS6AndUFS7>false</serviceSessionForUFS6AndUFS7>
            		<startSessionUFS7>true</startSessionUFS7>
           			<pathUFSToMigrate>/sm-uko/v2/session/create</pathUFSToMigrate>
        		</node>  
    		</nodes>
		</param>
		<param name="extendedPermission" description="">
   			<type>list</type>
			<nodes>
				<node id="ift-node1-mp.testonline.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="ift-node2-mp.testonline.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="ift-node4-mp.testonline.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="ift-node5-mp.testonline.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="mobile.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="10.21.152.7">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="greenfield1.online.sberbank.ru">
        			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="greenfield2.online.sberbank.ru">
        			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="node0.online.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="node1.online.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="node2.online.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="node3.online.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
      			<node id="node4.online.sberbank.ru">
         			<extendedPermissionEnabled>true</extendedPermissionEnabled>
         			<disabledPermissions>true</disabledPermissions>
      			</node>
   			</nodes>
		</param>
		<param name="SelfRegistrationCSAmApi" description="Включение mAPI на этапе саморегистрации в мобильном приложении">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="aim_withDeposit" description="Открытие цели с выбором типа вклада">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param description="" name="pushErib">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="EasyLogin" description="Включение новых правил создания логина">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="visa_tokenization_new" description="">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="invoicing_8.0" description="Инвойсинг">
			<type>service</type>
			<enabled>true</enabled>
		</param>
		<param name="non_accept_8.0" description="Безакцептное списание">
			<type>service</type>
			<enabled>true</enabled>
			<value>2000</value>
		</param>
        <param name="SpecialTutorialUID" description="Туториалы из списка 'специальные' и должны показываться при каждой регистрации">
              <tutorials>
                <tutorial UID="TutorialAnalyticsAgreement"/>
				<tutorial UID="TutorialIncognitoKey"/>
            	<tutorial UID="TutorialStatementsKey"/>
                <tutorial UID="TutorialStatementsKey23"/>
              </tutorials>
          </param>
		<param name="AllowedTutorialUID" description="Туториалы разрешенные к показу">
        	<tutorials>
                <tutorial UID="TutorialAnalyticsAgreement"/>
				<tutorial UID="TutorialIncognitoKey"/>
            	<tutorial UID="TutorialStatementsKey"/>
        	</tutorials>
		</param>
    	<param name="SpecialTutorialUID_v2" description="Туториалы из списка 'специальные' и должны показываться при каждой регистрации">
              <tutorials>
                <tutorial UID="TutorialAnalyticsAgreement"/>
				<tutorial UID="TutorialIncognitoKey"/>
            	<tutorial UID="TutorialStatementsKey"/>
              </tutorials>
        </param>
		<param name="AllowedTutorialUID_v2" description="Туториалы разрешенные к показу">
        	<tutorials>
                <tutorial UID="TutorialAnalyticsAgreement"/>
				<tutorial UID="TutorialIncognitoKey"/>
            	<tutorial UID="TutorialStatementsKey"/>
        	</tutorials>
		</param>
		<param name="iOSAppDesing" description="Парамтеры iOS App Design">
			<registrationLicenceLink>http://www.sberbank.ru/common/img/uploaded/files/pdf/policy.pdf</registrationLicenceLink>
            <p2pMaxLimit>1000000</p2pMaxLimit>
            <specialP2PMaxLimit>5000000</specialP2PMaxLimit>
          	<accountNumber>true</accountNumber>
          	<registrationPrimaryFlowByCardNumber>true</registrationPrimaryFlowByCardNumber>
          	<regNotSberbankCardError>true</regNotSberbankCardError>
          	<abTests>true</abTests>
          	<autofillEnabled>true</autofillEnabled>
          	<siriShortcutsEnabled>true</siriShortcutsEnabled>
          	<combinedRegistration>true</combinedRegistration>
          	<sberIDRegFirstScreen>true</sberIDRegFirstScreen>
          	<sberIDRegAndAuth>true</sberIDRegAndAuth>
          	<newFocusStyle>true</newFocusStyle>
          	<newTextsForRegistrationEnabled>true</newTextsForRegistrationEnabled>
          	<requestAnalyticsEnabled>true</requestAnalyticsEnabled>
          	<depositPromoBanner>
              	<enabled>false</enabled>
				<closeButtonEnabled>true</closeButtonEnabled>
				<version>1</version>
              	<title>Открыть вклад</title>
              	<description>На выгодных условиях</description>
              	<backgroundColor>0xF1F3FC</backgroundColor>
			</depositPromoBanner>
            <imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
		</param>
		<param name="iOSPlatform" description="Парамтеры iOS Platform">
			<loaderRequestAdapterEnabled>true</loaderRequestAdapterEnabled>
          	<servicesPaymentsEnabled>true</servicesPaymentsEnabled>
          	<appPermissionsAnalyticsEnabled>true</appPermissionsAnalyticsEnabled>
        	<operationsScreenMid2019Enabled>true</operationsScreenMid2019Enabled>
      	</param>
      	<param name="geoservice" description="Настройка URL гео-сервисов для блоков">
			<type>list</type>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<host>https://geo-t.online.sberbank.ru/</host>
                  	<yandexMapExperiment>false</yandexMapExperiment>
				</node>
				<node id="node1.online.sberbank.ru">
					<host>https://geo-t.online.sberbank.ru/</host>
                  	<yandexMapExperiment>false</yandexMapExperiment>
				</node>
                <node id="node2.online.sberbank.ru">
					<host>https://geo-t.online.sberbank.ru/</host>
                  	<yandexMapExperiment>false</yandexMapExperiment>
				</node>
				<node id="node3.online.sberbank.ru">
					<host>https://geo-t.online.sberbank.ru/</host>
                  	<yandexMapExperiment>false</yandexMapExperiment>
				</node>
				<node id="node4.online.sberbank.ru">
					<host>https://geo-t.online.sberbank.ru/</host>
                  	<yandexMapExperiment>false</yandexMapExperiment>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<host>https://geo1.online.sberbank.ru/</host>
                    <yandexMapExperiment>true</yandexMapExperiment>
				</node>
				<node id="greenfield2.online.sberbank.ru">
					<host>https://geo-t.online.sberbank.ru/</host>
                  	<yandexMapExperiment>true</yandexMapExperiment>
				</node>
              <node id="mobile.sberbank.ru" description="Стенд ПСИ">
                    <host>https://geo-t.online.sberbank.ru:1112/</host>
                	<yandexMapExperiment>true</yandexMapExperiment>
              </node>
              <node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
					<host>https://geo-t.online.sberbank.ru/</host>
                	<yandexMapExperiment>true</yandexMapExperiment>
              </node>
              <node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
                    <host>https://geo-t.sberbank.ru/</host>
                	<yandexMapExperiment>true</yandexMapExperiment>
              </node>
              <node id="psinode2.testonline.sberbank.ru">
                    <host>https://geo-t.online.sberbank.ru:1112/</host>
                	<yandexMapExperiment>true</yandexMapExperiment>
              </node>
           </nodes>
		</param>

      	<param name="lastToggleV2" description="Уведомление о принудительном обновлении в МП">
    		<enabled>true</enabled>
    		<lastToggleVerstion>9.5</lastToggleVerstion>
    		<lastToggleDate>1639129600</lastToggleDate>
          	<appStoreLink>https%3A%2F%2Fitunes.apple.com%2Fru%2Fapp%2F%25D1%2581%25D0%25B1%25D0%25B5%25D1%2580%25D0%25B1%25D0%25B0%25D0%25BD%25D0%25BA-%25D0%25BE%25D0%25BD%25D0%25BB%25D0%25B0%25D0%25B9%25D0%25BD%2Fid492224193%3Fmt%3D8</appStoreLink>
          	<appWebLink>https%3A%2F%2Fonline.sberbank.ru%2FCSAFront%2Findex.do</appWebLink>
          	<lastToggleSDK>9.0</lastToggleSDK>
          	<lastTogglePeriod>0</lastTogglePeriod>
          	<lastToggleDevice>
              	<device>iPhone</device>
              	<device>iPhone 3G</device>
              	<device>iPhone 3GS</device>
              	<device>iPhone 4</device>
          	</lastToggleDevice>
    		<messageText>Вышла новая версия приложения. Чтобы вам было доступно еще больше услуг, обновите приложение через AppStore.</messageText>
          	<upMessageText>Версия приложения устарела и больше не работает. Чтобы воспользоваться приложением:
1. Обновите операционную систему: зайдите в Настройки – Основные – Обновление ПО – Установить.
2. После этого обновите приложение до рабочей версии.</upMessageText>
   			<errorText>Версия приложения устарела и больше не работает. Чтобы воспользоваться приложением, его нужно обновить через AppStore.</errorText>
          	<fatalErrorText>Версия приложения устарела и больше не поддерживается на вашем телефоне. Вы можете использовать сайт Сбербанк Онлайн.</fatalErrorText>
		</param>
      	<param name="signOnParams" description="Парамтеры стрима SignOn">
            <type>list</type>
            <offerNonAccept>http://www.sberbank.ru/common/img/uploaded/files/pdf/usloviya_perevoda.pdf</offerNonAccept>
          	<merchantDataManagementServiceName>Управление Сбербанк ID</merchantDataManagementServiceName>
   			<nodes>
   		 		<node id="node0.online.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                  	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="node1.online.sberbank.ru">
     				<qrPayments>true</qrPayments>
                    <qrP2P>true</qrP2P>
                    <qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="node2.online.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="node3.online.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="greenfield1.online.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="greenfield2.online.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
                <node id="194.186.207.23">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="ift-node1.testonline.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="ift-node2.testonline.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                  	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="ift-node1-mp.testonline.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                   	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="ift-node2-mp.testonline.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>true</qrP2P>
                  	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
    			<node id="mobile.sberbank.ru">
     				<qrPayments>true</qrPayments>
                   	<qrP2P>false</qrP2P>
                  	<qrMerchantBinding>true</qrMerchantBinding>
                    <universalLinks>true</universalLinks>
					<invoicing>true</invoicing>
					<nonAccept>
						<enabled>true</enabled>
						<value>2000</value>
					</nonAccept>
                  	<merchantDataManagement>true</merchantDataManagement>
    			</node>
   			</nodes>
        </param>
		<param name="aim_withCurrency" description="Открытие валютных целей">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
    	<param name="offersAndStories" description="Предложения продуктов и истории на витринах продаж">
        	<type>list</type>
			<enabled>true</enabled>
			<nodes>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
                          	<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                  	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
                  	<marketplaceStories>
						<enabled>true</enabled>
						<limit>214748364</limit>
						<closed>false</closed>
						<opened>false</opened>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>7</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</marketplaceStories>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardPayment</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
                          	<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                  	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<marketplaceStories>
						<enabled>true</enabled>
						<limit>214748364</limit>
						<closed>false</closed>
						<opened>false</opened>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>7</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</marketplaceStories>                	
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>1</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>RUB</currencyCode>
                      	<classificationCodes>
                      		<classificationCode>1678</classificationCode>
                          	<classificationCode>1555</classificationCode>
                          	<classificationCode>2222</classificationCode>
                      	</classificationCodes>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
                    	<mvpEnabled>true</mvpEnabled>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                 	<marketplaceStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>7</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</marketplaceStories>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>1</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>15</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>1</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>false</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<mainScreenStories>
						<enabled>false</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>false</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>20</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                 	<marketplaceStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>7</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</marketplaceStories>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>1</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>RUB</currencyCode>
                      	<classificationCodes>
                      		<classificationCode>1678</classificationCode>
                          	<classificationCode>1555</classificationCode>
                          	<classificationCode>2222</classificationCode>
                      	</classificationCodes>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>15</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>1</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>false</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>0</preloadCount>
                    	<lifetimeOfCache>10</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<marketplaceStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>7</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</marketplaceStories>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                          	<formName>ExtCardPayment</formName>
                      	</formNames>
                      	<minSumRUB>1</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>RUB</currencyCode>
                      	<classificationCodes>
                      		<classificationCode>5691</classificationCode>
                          	<classificationCode>1555</classificationCode>
                          	<classificationCode>2222</classificationCode>
                      	</classificationCodes>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>10</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>15</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>1</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>false</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>5</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<mainScreenStories>
						<enabled>false</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>false</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>20</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                 	<marketplaceStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>7</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</marketplaceStories>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>1</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>RUB</currencyCode>
                      	<classificationCodes>
                      		<classificationCode>1678</classificationCode>
                          	<classificationCode>1555</classificationCode>
                          	<classificationCode>2222</classificationCode>
                      	</classificationCodes>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>20</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>0</preloadCount>
						<lifetimeOfCache>10</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>false</enabled>
						<limit>214748364</limit>
                      	<title>Предложения</title>
						<closed>false</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>15</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>false</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Истории</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>0</preloadCount>
                    	<lifetimeOfCache>10</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>3</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
                      	<likeButtonIsDisabled>false</likeButtonIsDisabled>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>20</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardPayment</formName>
                      	</formNames>
                      	<minSumRUB>-5000</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>RUB</currencyCode>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
              <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>0</preloadCount>
						<lifetimeOfCache>10</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>false</enabled>
						<limit>214748364</limit>
                      	<title>Предложения</title>
						<closed>false</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
                  	<mainScreenSberKids>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenSberKids>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>15</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Истории</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>0</preloadCount>
                    	<lifetimeOfCache>10</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>3</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
                      	<likeButtonIsDisabled>false</likeButtonIsDisabled>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>20</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardPayment</formName>
                      	</formNames>
                      	<minSumRUB>-5000</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>RUB</currencyCode>
                  	</paymentsHistoryScreen>
                    <premierOffersScreen>
                        <enabled>true</enabled>
                        <limit>20</limit>
                    </premierOffersScreen>
                    <premierPrivilegesScreen>
					    <enabled>true</enabled>
                        <limit>20</limit>
                    </premierPrivilegesScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>20160</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>20160</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>1</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>15</limit>
						<title>Рекомендуем</title>
            			<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                        <sectionEnabled>true</sectionEnabled>
						<closed>false</closed>
						<opened>false</opened>
                    	<mvpEnabled2>false</mvpEnabled2>
                      	<lifetimeOfCache>20160</lifetimeOfCache>
                      	<cache>true</cache>
                      	<lifetimeOfCachePermissions>20160</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>1</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardPayment</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>100</termDays>
                      	<currencyCode>RUB</currencyCode>
                  	</paymentsHistoryScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardPayment</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardTransferIn</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
                <node id="node4.online.sberbank.ru">
					<enabled>true</enabled>
                  	<settings>
						<cache>
							<lifetimeOfIcons>129600</lifetimeOfIcons>
							<lifetimeOfImages>20160</lifetimeOfImages>
                          	<lifetimeOfVideo>3</lifetimeOfVideo>
						</cache>
					</settings>
                  	<mainScreenHeader>
						<enabled>true</enabled>
						<limit>6</limit>
						<tabTitle>Истории</tabTitle>
						<preloadCount>1</preloadCount>
						<lifetimeOfCache>5</lifetimeOfCache>
						<cache>true</cache>
						<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
						<cachePermissions>true</cachePermissions>
                  	</mainScreenHeader>
					<mainScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>true</closed>
						<opened>false</opened>
					</mainScreen>
                  	<mainScreenDeposits>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenDeposits>
                  	<mainScreenLoans>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenLoans>
                  	<mainScreenCards>
						<enabled>true</enabled>
						<limit>1</limit>
                      	<bottomPosition>false</bottomPosition>
					</mainScreenCards>
					<successScreen>
						<enabled>true</enabled>
						<limit>2147483647</limit>
					</successScreen>
					<mainScreenStories>
						<enabled>true</enabled>
						<limit>2147483647</limit>
						<closed>false</closed>
						<opened>false</opened>
                      	<sectionEnabled>true</sectionEnabled>
                      	<tabTitle>Советы</tabTitle>
                    	<title>Рекомендуем</title>
						<no_offers_text>Для вас пока нет рекомендаций, но они скоро появятся</no_offers_text>
                      	<preloadCount>1</preloadCount>
                    	<lifetimeOfCache>5</lifetimeOfCache>
    					<cache>true</cache>
    					<lifetimeOfCachePermissions>2</lifetimeOfCachePermissions>
    					<cachePermissions>true</cachePermissions>
					</mainScreenStories>
                	<mainScreenTutorial>
						<enabled>true</enabled>
						<limit>10</limit>
					</mainScreenTutorial>
                  	<paymentsHistoryScreen>
                      	<enabled>true</enabled>
                      	<limit>1</limit>
                      	<formNames>
                        	<formName>ExtCardPayment</formName>
                        	<formName>ExtCardOtherIn</formName>
                        	<formName>ExtCardCashIn</formName>
                      	</formNames>
                      	<minSumRUB>500</minSumRUB>
                      	<maxSumRUB>100000000</maxSumRUB>
                      	<termDays>365</termDays>
                      	<currencyCode>USD</currencyCode>
                  	</paymentsHistoryScreen>
                  	<promotionScreen>
					    <enabled>true</enabled>
                    </promotionScreen>
				</node>
			</nodes>
		</param>
		<param name="CardRegistrationApp" description="Включение регистрации устройства по номеру карты">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="LoginBirthdayRegistrationApp" description="Включение регистрации по логину и дате рождения">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="digitalCreditCustomers" description="Список серверов, за которыми закреплены клиенты, которым доступен конкретный функционал">
	        <type>list</type>
			<enabled>true</enabled>
          <versions>
            <version id="9.3">
            	<loanRequest>false</loanRequest>
            	<insuranceOnIssuance>false</insuranceOnIssuance>
            	<mainDeeplink>false</mainDeeplink>
                <loanRequestPreadopted>false</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.4">
            	<loanRequest>false</loanRequest>
            	<insuranceOnIssuance>false</insuranceOnIssuance>
            	<mainDeeplink>false</mainDeeplink>
                <loanRequestPreadopted>false</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.4.1">
            	<loanRequest>false</loanRequest>
            	<insuranceOnIssuance>false</insuranceOnIssuance>
            	<mainDeeplink>false</mainDeeplink>
                <loanRequestPreadopted>false</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.5">
            	<loanRequest>false</loanRequest>
            	<insuranceOnIssuance>false</insuranceOnIssuance>
            	<mainDeeplink>false</mainDeeplink>
                <loanRequestPreadopted>false</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.6">
            	<loanRequest>true</loanRequest>
            	<insuranceOnIssuance>true</insuranceOnIssuance>
                <mainDeeplink>true</mainDeeplink>
                <loanRequestPreadopted>false</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.7">
            	<loanRequest>true</loanRequest>
            	<insuranceOnIssuance>true</insuranceOnIssuance>
                <mainDeeplink>true</mainDeeplink>
                <loanRequestPreadopted>false</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.8">
            	<loanRequest>true</loanRequest>
            	<insuranceOnIssuance>true</insuranceOnIssuance>
            	<mainDeeplink>true</mainDeeplink>
                <loanRequestPreadopted>true</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.9">
            	<loanRequest>true</loanRequest>
            	<insuranceOnIssuance>true</insuranceOnIssuance>
            	<mainDeeplink>true</mainDeeplink>
                <loanRequestPreadopted>true</loanRequestPreadopted>
                <insuranceOnRequest>false</insuranceOnRequest>
          	</version>
            <version id="9.10">
            	<loanRequest>true</loanRequest>
            	<insuranceOnIssuance>true</insuranceOnIssuance>
            	<mainDeeplink>true</mainDeeplink>
                <loanRequestPreadopted>true</loanRequestPreadopted>
                <insuranceOnRequest>true</insuranceOnRequest>
          	</version>
			<version id="9.13">
				<loanRequest>true</loanRequest>
				<insuranceOnIssuance>true</insuranceOnIssuance>
				<mainDeeplink>true</mainDeeplink>
				<loanRequestPreadopted>true</loanRequestPreadopted>
				<insuranceOnRequest>true</insuranceOnRequest>
				<loanRequestCreditCapacity>true</loanRequestCreditCapacity>
              	<CreditRequestInHistoryOperation>true</CreditRequestInHistoryOperation>
			</version>
            <version id="10.0">
				<loanRequest>true</loanRequest>
				<insuranceOnIssuance>true</insuranceOnIssuance>
				<mainDeeplink>true</mainDeeplink>
				<loanRequestPreadopted>true</loanRequestPreadopted>
				<insuranceOnRequest>true</insuranceOnRequest>
				<loanRequestCreditCapacity>true</loanRequestCreditCapacity>
              	<CreditRequestInHistoryOperation>true</CreditRequestInHistoryOperation>
			</version>
            <version id="10.1">
				<loanRequest>true</loanRequest>
				<insuranceOnIssuance>true</insuranceOnIssuance>
				<mainDeeplink>true</mainDeeplink>
				<loanRequestPreadopted>true</loanRequestPreadopted>
				<insuranceOnRequest>true</insuranceOnRequest>
				<loanRequestCreditCapacity>true</loanRequestCreditCapacity>
              	<loanKladrWidgetForShortForm>true</loanKladrWidgetForShortForm>
              	<CreditRequestInHistoryOperation>true</CreditRequestInHistoryOperation>
			</version>
            <version id="10.2">
				<loanRequest>true</loanRequest>
				<insuranceOnIssuance>true</insuranceOnIssuance>
				<mainDeeplink>true</mainDeeplink>
				<loanRequestPreadopted>true</loanRequestPreadopted>
				<insuranceOnRequest>true</insuranceOnRequest>
				<loanRequestCreditCapacity>true</loanRequestCreditCapacity>
              	<loanKladrWidgetForShortForm>true</loanKladrWidgetForShortForm>
              	<CreditRequestInHistoryOperation>true</CreditRequestInHistoryOperation>
			</version>
            <version id="default">
            	<loanRequest>true</loanRequest>
            	<insuranceOnIssuance>true</insuranceOnIssuance>
            	<mainDeeplink>true</mainDeeplink>
                <loanRequestPreadopted>true</loanRequestPreadopted>
                <insuranceOnRequest>true</insuranceOnRequest>
				<loanRequestCreditCapacity>true</loanRequestCreditCapacity>
              	<loanKladrWidgetForShortForm>true</loanKladrWidgetForShortForm>
                <CreditRequestInHistoryOperation>true</CreditRequestInHistoryOperation>
          </version>
        </versions>
		</param>
    	<param name="digitalCreditPostService" description="Параметры постпродажного кредитования">
    		<type>list</type>                       
    		<enabled>true</enabled>
    		<released>
        		<version id="default">
            		<enabled>true</enabled>
            		<sberAnalytica>true</sberAnalytica>
        		</version>
    		</released>                                   
		</param>
		<param name="DomClickMortgage" description="Mortgage application through DomClick mobile application">
            <type>list</type>
            <nodes>
                <node id="node0.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="node1.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="node2.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="node3.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="node4.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="greenfield1.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="greenfield2.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="mobile.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                </node>
            </nodes>
        </param>
		<param name="digitalCreditServices" description="Параметры сервисов функционала">
			<type>list</type>
			<enabled>true</enabled>
			<services>
				<service name="ufs.consumer.loan.v1" description="Сервис ЕФС">
					<host/>
					<path>consumer-loan/v2/mobile/banking/products/loans/consumerloan/request</path>
				</service>
				<service name="PersData" description="Текст виджета условий обработки ПДн">
					<host>https://185.157.96.21:443</host>
					<path>consumer-loan/v2/mobile/banking/products/loans/consumerloan/request/GetConfirmationAgreement/</path>
				</service>
                <service name="restForMain.v1">
                    <host/>
                    <path>consumer-loan/v1/mobile/banking/products/loans/requests/list</path>
                </service>
                <service name="deeplinkToMainFlow">
                    <version id="default">
                        <flow permission="LoanRequestWithInsuranceOnRequest">doActionWithRequestInsuranceDeepLink</flow>
                        <flow permission="UFSLoanRequestPreadopted">doActionPreadoptedDeepLink</flow>
                        <flow permission="UFSLoanRequestWithInsurance">doActionWithInsuranceDeepLink</flow>
                        <flow permission="UFSLoanRequest">doActionDeepLink</flow>  	
                    </version>
                 </service>
			</services>
		</param>
		<param name="CoreAddress" description="Адрес хоста и путь к веб сервису КЛАДР">
			<type>service</type>
			<enabled>true</enabled>
			<services>
				<service name="ufs.kladr.v1">
					<path>/loan-suggestion/services/rest/v2/SBOL/Suggestions.KLADR</path>
				</service>
				<service name="ufs.kladr.v2">
					<path>/loan-suggestion/services/rest/v2/mobile/Suggestions.KLADR</path>
				</service>
				<service name="ufs7.kladr.v1">
					<path>/loan-suggestion/services/rs/Suggestions.KLADR</path>
				</service>
              <service name="ufs.kladr.UFS7">
                    <path>/loan-suggestion/services/rs/Suggestions.KLADR</path>
              </service>
			</services>
,		</param>
		<param name="shouldShowCreditCapacityScale" description="Отображение шкалы кредитного потенциала в процессе оформления кредитной карты">
			<type>service</type>
			<enabled>true</enabled>
		</param>
        <param name="creditCardOrder" description="Заказ кредитной карты в ЕФС">
			<type>service</type>
			<enabled>true</enabled>
		</param>
      	<param name="creditCardOrderV2" description="Заказ кредитной карты в ЕФС, версия 2">
			<type>service</type>
   			<enabled>true</enabled>
		</param>
        <param name="digitalCreditCardOrder" description="Заказ цифровой кредитной карты в ЕФС">
			<type>service</type>
   			<enabled>true</enabled>
		</param>
        <param name="creditCardDynamicFields" description="Динамические поля на экране с информацией по кредитной карте при заказе в ЕФС">
			<type>service</type>
   			<enabled>true</enabled>
		</param>
        <param name="bannerManagement" description="Управление содержимым баннера">
			<type>list</type>
			<enabled>true</enabled>
			<icon>card</icon>
			<title>Заявка на кредитную карту</title>
            <subtitle>0 руб. за обслуживание&#xA;без дополнительных условий</subtitle>
		</param>
    <param name="deactivationGhostAccount" description="Управление отображением гост-аккаунта на кредитную карту">
      <enabled>false</enabled>
      <nodes>
          <node id="mobile.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node4.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
              <enabled>false</enabled>
          </node>
          <node id="greenfield2.online.sberbank.ru">
              <enabled>false</enabled>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="ift-node5.testonline.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="ift-node5-mp.testonline.sberbank.ru">
              <enabled>true</enabled>
          </node>
      </nodes>
  </param>
      	<param name="GetDoc" description="Кредитная карта подробности тарифа">
			<type>list</type>
			<enabled>true</enabled>
			<services>
				<service name="GetDoc" description="">
				<host>https://pfl-efs.sigma.sbrf.ru:443</host>
				<path>/credit-cards/short-form-capacity/v1/mobile/banking/product/ccard/short-ccard-request/getTextOfCardDetailsInfo</path>
			</service>
		</services>
		</param>
      	<param name="creditCardUfsHistory" description="Отображение подробностей по заказу кредитной карты ЕФС в ИО">
			<type>service</type>
   			<enabled>true</enabled>
		</param>
		<param name="creditCardOrderServices" description="Параметры сервисов функционала заказа кредитной карты в ЕФС">
			<type>list</type>
			<enabled>true</enabled>
			<services>
				<service name="persDataAgreement" description="Текст виджета условий обработки персональных данных">
					<host>https://pfl-psi.efstst.sigma.sbrf.ru:443</host>
					<path>/credit-cards/short-form-capacity/v1/mobile/banking/product/ccard/short-ccard-request/getTextOfAgreementOnTransferInfo</path>
				</service>
			</services>
		</param>
      	<param name="PushPlatformID" description="URL серверов Push-платформы">
    		<type>setting</type>
        	<enabled>true</enabled>
            <platforms>
				<platform id="1" url="http://pushservertest.mfms.ru/push-test"/>
            	<platform id="3" url="https://pushserver.mfms.ru/sbrf"/>
            	<platform id="4" url="https://pushserver.sberbank-tele.com"/>
            	<platform id="5" url="https://pushserver-test.sberbank-tele.com"/>
                <platform id="6" url="https://pushmarketing.sberbank-tele.com"/>
            </platforms>
		</param>
      	<param name="StatementsAndReferencesEntryPoint" description="Справки и выписки c v9.3 и более">
			<type>list</type>
			<enabled>true</enabled>
			<old_entry>false</old_entry>
        <nodes>
	        <node id="node0.online.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="node1.online.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="node2.online.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="node3.online.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="greenfield1.online.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="greenfield2.online.sberbank.ru">
	            <enabled>false</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="mobile.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="ift-node1.testonline.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="ift-node2.testonline.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="ift-node1-mp.testonline.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="ift-node2-mp.testonline.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>false</statementBinaryFile>
	        </node>
	        <node id="ift-node5-mp.testonline.sberbank.ru">
	            <enabled>true</enabled>
	            <statementsHistory>true</statementsHistory>
				<old_entry>false</old_entry>
				<statementsSmartSearch>true</statementsSmartSearch>
				<statementsPeriodLimit>true</statementsPeriodLimit>
				<statementBinaryFile>true</statementBinaryFile>
	        </node>
	    </nodes>
		</param>
      	<param name="StatementsAndReferences" description="Справки и выписки c v8.11">
			<type>list</type>
        <nodes>
	        <node id="node0.online.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="node1.online.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="node2.online.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="node3.online.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="greenfield1.online.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="greenfield2.online.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="mobile.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="ift-node1.testonline.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="ift-node2.testonline.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	        <node id="ift-node1-mp.testonline.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
	            <statementsHistory>true</statementsHistory>
	        </node>
	    </nodes>
		</param>
      	<param name="StaticSourceMerchantPics" description="статресурс для логотипов">
    		<type>source</type>
    		<link>https://enricher.mfms.ru/merchantIcons/</link>
		</param>
        <param name="CarLoanRequest" description="Заявка на автокредит с версии 9.3">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      <param name="CarLoan" description="Заявка на автокредит">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
      	<param name="CarLoansOperationHistory" description="Работа с историей операций">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
        <param name="CarLoansDetails2" description="Детализация автокредита">
        	<type>setting</type>
        	<enabled>true</enabled>
        </param>      
      	<param name="CarLoansPayment" description="Пополнение счета по автокредиту">
			<type>setting</type>
			<enabled>true</enabled>
			<refillProvider>622344</refillProvider>
        <param name="CarLoansDeeplink" description="Диплинк">
        	<type>setting</type>
        	<enabled>true</enabled>
        </param>
		</param>
       <param name="CarLoansTutorial" description="Отображение туториала">
      		<type>setting</type>
       		<enabled>true</enabled>
       </param>
      <param name="CarLoansRus" description="Ввод марок/моделей на русском">
        	<type>setting</type>
        	<enabled>true</enabled>
        	<URL>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/CarLoansRus.json</URL>
      </param>
      <param name="CarLoansAutoPay" description="Доступность автоплатежа из детализации АК">
        	<type>setting</type>
        	<enabled>true</enabled>
      </param>
        <param name="CarLoanServices" description="Параметры сервисов функционала">
            <type>list</type>
            <enabled>true</enabled>
            <services>
                <service name="PersData" description="Текст виджета условий обработки ПДн">
                <path>/person-credit-mb/v1/mobile/Banking/Products/Loans/CarLoans/Application/GetAgreement</path>
                </service>
            </services>
        </param>
		<param name="WelfareProductsMainScreen" description="Продукты благосостояния на главном экране">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="WelfareTutorial" description="Туториал на фичу">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
		<param name="WelfareProductsDetails" description="Карточки продуктов благосостояния (детализация продукта)">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="welfareProducts" description="Продукты благосостояния">
			<type>list</type>
			<enabled>true</enabled>
			<nodes>
				<node id="greenfield1.online.sberbank.ru">
					<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                 	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="194.186.207.23">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="mobile.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
              	<node id="node0.online.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="node1.online.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="node2.online.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="node3.online.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                    <isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="ift-node5.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="ift-node7.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                 	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
                <node id="ift-node7-mp.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                 	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="10.21.152.7">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
				<node id="msv-node2.testonline.sberbank.ru">
                  	<isShowInFinance>true</isShowInFinance>
                  	<isShowInFinancev2>true</isShowInFinancev2>
					<actionInvestmentsBuy>true</actionInvestmentsBuy>
					<actionPIF>true</actionPIF>
                  	<actionIPP>true</actionIPP>
                  	<autopaymentIPP>true</autopaymentIPP>
				</node>
			</nodes>
		</param>
		<param name="ContractListv2.1" description="Версия сервиса ContractList 2.1">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
      	<param name="UfsInsuranceMain" description="Отображение действующих страховых полисов на главной">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="UfsInsuranceMainContractsDetails" description="Отображение детальной информации по действующим страховым полисам на главной">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
        <param name="UfsInsuranceMainTurorial" description="Отображение туториала по страховкам">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="UfsInsuranceContracts" description="Список страховых контрактов и детальной информации по ним">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
  		<param name="UfsInsuranceSalesEnabled" description="Продажа страховых продуктов">
			<type>list</type>
			<enabled>true</enabled>
			<nodes>
				<node id="greenfield1.online.sberbank.ru">
					<UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="194.186.207.23">
                  	<UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="mobile.sberbank.ru">
                  	<UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
              	<node id="node0.online.sberbank.ru">
                  	<UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="node1.online.sberbank.ru">
                  <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="node2.online.sberbank.ru">
                  <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="node3.online.sberbank.ru">
                  <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="ift-node5.testonline.sberbank.ru">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                  <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
                	<UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="10.21.152.7">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
				<node id="msv-node2.testonline.sberbank.ru">
                   <UfsInsuranceSalesIpotekaInsEnabled>true</UfsInsuranceSalesIpotekaInsEnabled>
				</node>
			</nodes>
		</param>
        <param name="UfsInsuranceHistory" description="История операций по Страховым продуктам">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="UfsInvestmentsBuyShareHistory" description="История операций по докупке ПИФ">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
     	<param name="UfsInvestmentIIABuyCommonHistory" description="Переход из Истории операций к деталям операции по Пополнению ИИС/ДУ">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="UfsPensionPaymentIppHistory" description="История операций по пополнению ИПП">
          	<type>setting</type>
          	<enabled>true</enabled>
      	</param>
		<param name="UfsRurPayment" description="классические переводы в ЕФС, замена переводов ЕРИБа">
			<type>service</type>
			<enabled>true</enabled>
		</param>
		<param name="AccountSpecialCondition" description="Специальные условия по вкладу. Ограничение на максимальную сумму">
			<type>setting</type>
			<enabled>true</enabled>
	   </param>
       <param name="AccountSpecialConditionSum" description="Максимальное значение первоначального взноса, с которого начинает действовать пониженный процент по вкладу">
				<currencies>
					<currency>
						<id>RUB</id>
						<maxamount>100000</maxamount>
					</currency>
					<currency>
						<id>OTHER</id>
						<maxamount>0</maxamount>
					</currency>
				</currencies>
		</param>
		<param name="UiCaseGibddPenaltySearch" description="Уникальный пользовательский сценарий для поиска штрафов по ВУ/СТС">
			<type>list</type>
              <nodes>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
					<serviceID>688079</serviceID>
					<targetService>688457</targetService>
					<targetBilling>344</targetBilling>
					<targetProvider>688457</targetProvider>
				</node>
            	<node id="ift-node1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>624234</serviceID>
                  <targetService>627324</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>627324</targetProvider>
            	</node>
            	<node id="ift-node2.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>1146166</serviceID>
                  <targetService>626902</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>626902</targetProvider>
            	</node>
                <node id="ift-node5.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>623250</serviceID>
                  <targetService>625861</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>625861</targetProvider>
            	</node>
            	<node id="ift-node1-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>624234</serviceID>
                  <targetService>627324</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>627324</targetProvider>
            	</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>624234</serviceID>
                  <targetService>623095</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>623095</targetProvider>
            	</node>
            	<node id="ift-node2-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>623567</serviceID>
                  <targetService>626902</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>626902</targetProvider>
            	</node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>623250</serviceID>
                  <targetService>625861</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>625861</targetProvider>
            	</node>
                <node id="ift-node7-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>618157</serviceID>
                  <targetService>626170</targetService>
                  <targetBilling>344</targetBilling>
                  <targetProvider>626170</targetProvider>
            	</node> 
            	<node id="node3.online.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>500202753</serviceID>
                  <targetService>500413146</targetService>
                  <targetBilling>284</targetBilling>
                  <targetProvider>500413146</targetProvider>
            	</node>
            	<node id="node2.online.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>500204565</serviceID>
                  <targetService>500413943</targetService>
                  <targetBilling>284</targetBilling>
                  <targetProvider>500413943</targetProvider>
            	</node>
            	<node id="node1.online.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>387491</serviceID>
                  <targetService>596879</targetService>
                  <targetBilling>284</targetBilling>
                  <targetProvider>596879</targetProvider>
            	</node>
            	<node id="greenfield1.online.sberbank.ru">
                  <enabled>true</enabled>
                  <serviceID>500202753</serviceID>
                  <targetService>550445849</targetService>
                  <targetBilling>284</targetBilling>
                  <targetProvider>550445849</targetProvider>
            	</node>
            </nodes>
		</param>
		<param name="UiCaseGibddPenaltyPayByUin" description="Уникальный пользовательский сценарий для оплаты штрафов по УИН">
   			<type>list</type>
             <nodes>
               <node id="node0.online.sberbank.ru">
                    <enabled>false</enabled>
                    <serviceID>500204118</serviceID>
                    <targetService>500414394</targetService>
                    <targetBilling>284</targetBilling>
                    <targetProvider>500414394</targetProvider>
                </node>
                <node id="node1.online.sberbank.ru">
                    <enabled>false</enabled>
                    <serviceID>387492</serviceID>
                    <targetService>596878</targetService>
                    <targetBilling>284</targetBilling>
                    <targetProvider>596878</targetProvider>
                </node>
                <node id="node2.online.sberbank.ru">
                    <enabled>false</enabled>
                    <serviceID>500204566</serviceID>
                    <targetService>500413942</targetService>
                    <targetBilling>284</targetBilling>
                    <targetProvider>500413942</targetProvider>
                </node>
                <node id="node3.online.sberbank.ru">
                    <enabled>false</enabled>
                    <serviceID>500202754</serviceID>
                    <targetService>500413145</targetService>
                    <targetBilling>284</targetBilling>
                    <targetProvider>500413145</targetProvider>
                </node>
                <node id="node4.online.sberbank.ru">
                    <enabled>false</enabled>
                    <serviceID>500202754</serviceID>
                    <targetService>550445848</targetService>
                    <targetBilling>284</targetBilling>
                    <targetProvider>550445848</targetProvider>
                </node>
                <node id="greenfield1.online.sberbank.ru">
                    <enabled>false</enabled>
                    <serviceID>500202754</serviceID>
                    <targetService>550445848</targetService>
                    <targetBilling>284</targetBilling>
                    <targetProvider>550445848</targetProvider>
                </node>
				<node id="mobile.sberbank.ru">
					<enabled>false</enabled>
					<serviceID>222222</serviceID>
					<targetService>688092</targetService>
					<targetBilling>344</targetBilling>
					<targetProvider>688092</targetProvider>
			   </node>
               <node id="ift-node1.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>617948</serviceID>
                   <targetService>627335</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>627335</targetProvider>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>618120</serviceID>
                   <targetService>626914</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>626914</targetProvider>
                </node>
               	<node id="ift-node5.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>618157</serviceID>
                   <targetService>625837</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>625837</targetProvider>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>617948</serviceID>
                   <targetService>627335</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>627335</targetProvider>
                </node>
               <node id="ift-node0-mp.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>617948</serviceID>
                   <targetService>621822</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>621822</targetProvider>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>618120</serviceID>
                   <targetService>626914</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>626914</targetProvider>
                </node>
               	<node id="ift-node5-mp.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>618157</serviceID>
                   <targetService>625837</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>625837</targetProvider>
                </node>
               	<node id="ift-node7-mp.testonline.sberbank.ru">
                   <enabled>false</enabled>
                   <serviceID>623250</serviceID>
                   <targetService>626167</targetService>
                   <targetBilling>344</targetBilling>
                   <targetProvider>626167</targetProvider>
                </node>
              </nodes>
		</param>
      	<param name="EribGibddInfoService" description="Идентификаторы информационной услуги ГИБДД">
   			<nodes>
                <node id="ift-node1-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
                  	<targetBilling>344</targetBilling>
         			<targetService>627305</targetService>
         			<targetProvider>627305</targetProvider>
      			</node>
      			<node id="ift-node2-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
                  	<targetBilling>344</targetBilling>
         			<targetService>626860</targetService>
         			<targetProvider>626860</targetProvider>
      			</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
                  	<targetBilling>344</targetBilling>
         			<targetService>626141</targetService>
         			<targetProvider>626141</targetProvider>
      			</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
                  	<targetBilling>344</targetBilling>
         			<targetService>626096</targetService>
         			<targetProvider>626096</targetProvider>
      			</node>
      			<node id="mobile.sberbank.ru">
         			<enabled>false</enabled>
                  	<targetBilling>344</targetBilling>
         			<targetService>703227</targetService>         			
         			<targetProvider>703227</targetProvider>
      			</node>
              	<node id="psinode1.testonline.sberbank.ru">
                    <enabled>false</enabled>
                    <targetBilling>344</targetBilling>
         			<targetService>703227</targetService>
         			<targetProvider>703227</targetProvider>
                </node> 
   			</nodes>
		</param>
     	<param name="EribGibddPushDetailService" description="Идентификаторы услуги оплаты штрафа ГИБДД из пуша">
   			<nodes>
      			<node id="ift-node1-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
         			<targetBilling>344</targetBilling>
         			<targetService>627304</targetService>
         			<targetProvider>627304</targetProvider>
      			</node>
      			<node id="ift-node2-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
         			<targetBilling>344</targetBilling>
         			<targetService>626859</targetService>
         			<targetProvider>626859</targetProvider>
      			</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
         			<targetBilling>344</targetBilling>
         			<targetService>626859</targetService>
         			<targetProvider>626859</targetProvider>
      			</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
         			<enabled>true</enabled>
         			<targetBilling>344</targetBilling>
         			<targetService>626095</targetService>
         			<targetProvider>626095</targetProvider>
      			</node>
   			</nodes>
		</param>
      	<param name="PaymentTaxesLkFns" description="Интеграция ЛК ФНС и МП СБОЛ">
 			<enabled>true</enabled>
		</param>
    	<param name="EribGibddSixthStatus" description="Недоступные к оплате штрафы из системы Автокод">
    		<enabled>false</enabled>
    		<nodes>
        		<node id="ift-node1-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
        		<node id="ift-node2-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
              	<node id="ift-node3-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
              	<node id="ift-node4-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
              	<node id="ift-node6-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
              	<node id="mobile.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
    		</nodes>
		</param>
    	<param name="PaymentTaxesNewCardAutoSelection" description="Автовыбор карты списания для оплаты налогов">
 			<enabled>true</enabled>
 			<nodes>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
   					<enabled>true</enabled>
  				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
   					<enabled>true</enabled>
  				</node>
              	<node id="ift-true-mp.testonline.sberbank.ru">
   					<enabled>false</enabled>
  				</node>
              	<node id="ift-node3-mp.testonline.sberbank.ru">
   					<enabled>true</enabled>
  				</node>
              	<node id="ift-node2-mp.testonline.sberbank.ru">
   					<enabled>true</enabled>
  				</node>
              	<node id="ift-node1-mp.testonline.sberbank.ru">
   					<enabled>true</enabled>
  				</node>
 			</nodes>
		</param>
      	<param name="UiCaseGibddPenaltyClientProfileIntegration" description="Интеграция с ЕПК по документам ВУ/СТС">
    		<type>list</type>
    		<nodes>
              	<node id="ift-node1-mp.testonline.sberbank.ru">
        			<enabled>true</enabled>
        		</node>
              	<node id="ift-node3-mp.testonline.sberbank.ru">
        			<enabled>true</enabled>
        		</node>
        		<node id="ift-node5-mp.testonline.sberbank.ru">
        			<enabled>true</enabled>
        		</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
        			<enabled>true</enabled>
        		</node>
              	<node id="mobile.sberbank.ru">
        			<enabled>true</enabled>
        		</node>
    		</nodes>
		</param>
		<param name="creditCapacity" description="Кредитный потенциал ">
			<type>setting</type>
			<enabled>true</enabled>
          	<services>
				<service name="CapacityCalculationAgreement" description="Текст согласия клиента на обработку персональных данных для расчета КП">
					<path>/persDataAgreement/pdp-agreement/v1/CapacityCalculationAgreement.json</path>
                  	<description>Нажимая кнопку "Рассчитать", вы соглашаетесь с условиями <a>ПАО Сбербанк</a></description>
                  	<host>https://ift-stat.testonline.sberbank.ru:4463</host>
                	<path2>/PhizIC-res/Staticres/persDataAgreement/pdp-agreement/cp/v1/CapacityCalculationAgreement.html</path2>
				</service>
                <service name="CapacityConsumerRequestAgreement" description="Текст согласия клиента на подачу заявки на потребительский кредит">
					<path>/persDataAgreement/pdp-agreement/v1/CapacityConsumerRequestAgreement.json</path>
                    <description>Нажимая кнопку "Оформить", вы соглашаетесь с условиями <a>ПАО Сбербанк</a></description>
				</service>
			</services>
        	<nodes>
				<node id="node0.online.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="node1.online.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="node2.online.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="node3.online.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="greenfield1.online.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>false</CCOperationHistory>
				</node>
				<node id="greenfield2.online.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="194.186.207.23">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="mobile.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
				  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
             	<node id="10.21.152.7">
                  <enabled>true</enabled>
                  <enabled_v2>true</enabled_v2>
                  <calculateCC>true</calculateCC>
                  <showcase>true</showcase>
                  <createCreditIssue>true</createCreditIssue>
                  <creditCardApplication>true</creditCardApplication>
                  <CCTutorial>true</CCTutorial>
                  <CCOperationHistory>true</CCOperationHistory>
				</node>
			</nodes>
		</param>
        <param name="mobilePOS" description="Интернет кредитование">
	      <POSVersions>
            <version id="10.1">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="10.0">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.13">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.12">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.11">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.10.1">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.10">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.9">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="9.8">
                <enabled>true</enabled>
                <loanCalculator>true</loanCalculator>
              	<kladrEnabled>true</kladrEnabled>
            </version>
            <version id="default">
                <enabled>true</enabled>
                <loanCalculator>false</loanCalculator>
                <newStatusRoad>false</newStatusRoad>
            </version>
		 </POSVersions>
	  </param>
      <param name="creditCapacity_v2" description="Кредитный потенциал v9.5 и выше">
        <services>
            <service name="CapacityCalculationAgreement" description="Текст согласия клиента на обработку персональных данных для расчета КП">
              	<path>/person-credit/rest/v1/mobile/agreement/processing/static/CapacityCalculationAgreement.json</path>
            </service>
            <service name="CapacityConsumerRequestAgreement" description="Текст согласия клиента на подачу заявки на потребительский кредит">
                <path>/person-credit/rest/v1/mobile/agreement/processing/static/CapacityConsumerRequestAgreement.json</path>
            </service>
          	<service name="loanRequestCreditCapacity" description="URL Flow подачи кредитной заявки из витрины КП">
				<path>/consumer-loan/v2/mobile/banking/products/loans/consumerloan/request</path>
			</service>
        </services>
        <CCVersions>
		  <version id="9.10">
				<enabled>true</enabled>
				<calculateCC>true</calculateCC>
				<showcase>true</showcase>
				<loanApplication>true</loanApplication>
				<creditCardApplication>true</creditCardApplication>
				<CCTutorial>true</CCTutorial>
				<CCOperationHistory>true</CCOperationHistory>
				<calculateCCDeeplink>true</calculateCCDeeplink>
				<showcaseDeeplink>true</showcaseDeeplink>
				<flowVersions>
					<flowName name="form" version="0"/>
					<flowName name="loanRequest" version="0"/>
					<flowName name="operationHistory" version="0"/>
					<flowName name="default" version="0"/>
				</flowVersions>
		  </version>
          <version id="9.9">
				<enabled>true</enabled>
				<calculateCC>true</calculateCC>
				<showcase>true</showcase>
				<loanApplication>true</loanApplication>
				<creditCardApplication>true</creditCardApplication>
				<CCTutorial>true</CCTutorial>
				<CCOperationHistory>true</CCOperationHistory>
				<calculateCCDeeplink>true</calculateCCDeeplink>
				<showcaseDeeplink>true</showcaseDeeplink>
              	<flowVersions>
                  <flowName name="form" version="0"/>
                  <flowName name="loanRequest" version="0"/>
                  <flowName name="operationHistory" version="0"/>
                  <flowName name="default" version="0"/>
                </flowVersions>
			</version>
			<version id="9.8">
				<enabled>true</enabled>
				<calculateCC>true</calculateCC>
				<showcase>true</showcase>
				<loanApplication>true</loanApplication>
				<creditCardApplication>true</creditCardApplication>
				<CCTutorial>true</CCTutorial>
				<CCOperationHistory>true</CCOperationHistory>
				<calculateCCDeeplink>true</calculateCCDeeplink>
				<showcaseDeeplink>true</showcaseDeeplink>
			</version>
			<version id="9.7.1">
				<enabled>true</enabled>
				<calculateCC>true</calculateCC>
				<showcase>true</showcase>
				<loanApplication>true</loanApplication>
				<creditCardApplication>true</creditCardApplication>
				<CCTutorial>true</CCTutorial>
				<CCOperationHistory>true</CCOperationHistory>
				<calculateCCDeeplink>true</calculateCCDeeplink>
				<showcaseDeeplink>true</showcaseDeeplink>
			</version>
            <version id="9.7">
                <enabled>true</enabled>
                <calculateCC>true</calculateCC>
                <showcase>true</showcase>
                <loanApplication>true</loanApplication>
                <creditCardApplication>true</creditCardApplication>
                <CCTutorial>true</CCTutorial>
                <CCOperationHistory>true</CCOperationHistory>
                <calculateCCDeeplink>true</calculateCCDeeplink>
                <showcaseDeeplink>true</showcaseDeeplink>
            </version>
            <version id="9.6">
                <enabled>true</enabled>
                <calculateCC>true</calculateCC>
                <showcase>true</showcase>
                <loanApplication>true</loanApplication>
                <creditCardApplication>true</creditCardApplication>
                <CCTutorial>true</CCTutorial>
                <CCOperationHistory>true</CCOperationHistory>
                <calculateCCDeeplink>true</calculateCCDeeplink>
                <showcaseDeeplink>true</showcaseDeeplink>
            </version>
            <version id="9.5">
                <enabled>true</enabled>
                <calculateCC>true</calculateCC>
                <showcase>true</showcase>
                <loanApplication>true</loanApplication>
                <creditCardApplication>true</creditCardApplication>
                <CCTutorial>true</CCTutorial>
                <CCOperationHistory>true</CCOperationHistory>
                <calculateCCDeeplink>true</calculateCCDeeplink>
                <showcaseDeeplink>true</showcaseDeeplink>
            </version>
            <version id="default">
                <enabled>true</enabled>
                <calculateCC>true</calculateCC>
                <showcase>true</showcase>
                <loanApplication>true</loanApplication>
                <creditCardApplication>true</creditCardApplication>
                <CCTutorial>true</CCTutorial>
                <CCOperationHistory>true</CCOperationHistory>
                <calculateCCDeeplink>true</calculateCCDeeplink>
                <showcaseDeeplink>true</showcaseDeeplink>
                <flowVersions>
                  <flowName name="form" version="0"/>
                  <flowName name="loanRequest" version="0"/>
                  <flowName name="operationHistory" version="0"/>
                  <flowName name="default" version="0"/>
                </flowVersions>
            </version>
        </CCVersions>
		</param>
		<param name="ExternalLogin" description="Включение аутентификации через СБОЛ на внешних ресурсах">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
		<param name="ExternalLogin_v2" description="Включение аутентификации через СБОЛ на внешних ресурсах v8.9.1+">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="ExternalLoginPKCE" description="Включение входа через SBOL с использованием спецификации PKCE">
    		<type>setting</type>
    		<enabled>true</enabled>
		</param>
      	<param name="SberIdSeamlessAuth_v2" description="Включение функционала бесшовной аутентификации через СБОЛ">
    		<type>setting</type>
    		<enabled>true</enabled>
		</param>
      	<param name="SberIDNewClaims" description="Доработки по отображению списка передаваемых данных">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="SberIDReEntryFragment" description="Включение экрана повторного входа через SBOL">
			<type>setting</type>
			<enabled>false</enabled>
		</param>
      	<param name="SberIdPaymentAndData" description="Включение оплаты/входа через SBOL">
            <type>setting</type>
            <enabled>true</enabled>
          	<string>Сервис временно недоступен, приносим свои извинения.</string>
          	<errorTitle>Оплата не выполнена</errorTitle>
        </param>
		<param name="SberIDQRPayment_v3" description="Включение QR-оплаты для СБОЛ 9.13+">
			<type>setting</type>
			<enabled>true</enabled>
			<nodes>
				<node id="mobile.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="psinode2.testonline.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="psinode1.testonline.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru" description="Стенд ИФТ блок 1">
					<enabled>false</enabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru" description="Стенд ИФТ блок 2">
					<enabled>false</enabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
					<enabled>false</enabled>
                </node>
				<node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
					<enabled>false</enabled>
				</node>
				<node id="node0.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="node4.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
				<node id="greenfield2.online.sberbank.ru">
					<enabled>false</enabled>
				</node>
			</nodes>
		</param>
    <param name="SberIDQRPayment_v2_External" description="Включение QR-оплаты нативной камерой для СБОЛ 9.13+">
      <type>setting</type>
      <enabled>true</enabled>
      <nodes>
        <node id="mobile.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="psinode2.testonline.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="psinode1.testonline.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="ift-node1.testonline.sberbank.ru" description="Стенд ИФТ блок 1">
          <enabled>true</enabled>
        </node>
        <node id="ift-node2.testonline.sberbank.ru" description="Стенд ИФТ блок 2">
          <enabled>true</enabled>
        </node>
        <node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
          <enabled>true</enabled>
        </node>
        <node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
          <enabled>true</enabled>
        </node>
        <node id="node0.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="node1.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="node2.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="node3.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="node4.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="greenfield1.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
        <node id="greenfield2.online.sberbank.ru">
          <enabled>true</enabled>
        </node>
      </nodes>
    </param>
		<param name="P2PTransferByPhoneToOtherBank" description="Перевод в другие банки по номеру телефона через УЭК">
			<type>list</type>
            		<enabled>false</enabled>
			<CustomMessageLimitEnabled>false</CustomMessageLimitEnabled>
			<CustomMessageLimit>Обратите внимание! Доступный лимит для совершения операции составляет</CustomMessageLimit>
			<serviceProviders>
			  <serviceProvider name="Tinkoff" visibleName="Тинькофф Банк">
				<nodes>
					<node id="mobile.sberbank.ru">
						<targetBilling>344</targetBilling>
						<targetProvider>688468</targetProvider>
						<targetService>688468</targetService>
					</node>
					<node id="ift-node1-mp.testonline.sberbank.ru">
						<targetBilling>344</targetBilling>
						<targetProvider>623368</targetProvider>
						<targetService>623368</targetService>
					</node>
                    <node id="ift-node0-mp.testonline.sberbank.ru">
						<targetBilling>344</targetBilling>
						<targetProvider>623368</targetProvider>
						<targetService>623368</targetService>
					</node>
					<node id="ift-node2-mp.testonline.sberbank.ru">
						<targetBilling>344</targetBilling>
						<targetProvider>623368</targetProvider>
						<targetService>623368</targetService>
					</node>
					<node id="greenfield1.online.sberbank.ru">
						<targetBilling>284</targetBilling>
						<targetProvider>550478249</targetProvider>
						<targetService>550478249</targetService>
					</node>
					<node id="greenfield2.online.sberbank.ru">
						<targetBilling>284</targetBilling>
						<targetProvider>500439915</targetProvider>
						<targetService>500439915</targetService>
					</node>
					<node id="node1.online.sberbank.ru">
						<targetBilling>284</targetBilling>
						<targetProvider>629175</targetProvider>
						<targetService>629175</targetService>
					</node>
					<node id="node2.online.sberbank.ru">
						<targetBilling>284</targetBilling>
						<targetProvider>500446239</targetProvider>
						<targetService>500446239</targetService>
					</node>
					<node id="node3.online.sberbank.ru">
						<targetBilling>284</targetBilling>
						<targetProvider>500445546</targetProvider>
						<targetService>500445546</targetService>
					</node>
					<node id="node4.online.sberbank.ru">
						<targetBilling>284</targetBilling>
						<targetProvider>500439915</targetProvider>
						<targetService>500439915</targetService>
					</node>
				</nodes>
			  </serviceProvider>
			</serviceProviders>
		</param>
		<param name="ExternalTopUp" description="P2P Пополнение карты клиента с карты стороннего банка" >
			<!-- Описание доступно тут: Вход в операцию > Условия доступности функицонала (https:// https://sbtatlas.sigma.sbrf.ru/wiki/pages/viewpage.action?pageId=750161862#id-АналитикапофичепополнениякартыСбербанкаскартыдругогобанкавМПiOS-Входвоперацию) -->
			<type>service</type>
			<enabled>false</enabled>  <!-- Для отключения функционала в 9.8 можно удалить тэг или выставить значение false -->
			<enabled_10_1>true</enabled_10_1>
			<copecksInAmountDisabled>false</copecksInAmountDisabled>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="mobile.sberbank.ru">
					<!--"Главный" стенд (ПСИ)-->
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="ift-node3-mp.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="ift-node4-mp.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
				<node id="194.186.207.23">
					<enabled_10_1>true</enabled_10_1>
					<copecksInAmountDisabled>false</copecksInAmountDisabled>
				</node>
			</nodes>
		</param>
      		<param name="P2PTransferByPhoneToOtherBankSKB" description="Перевод в Совкомбанк по номеру телефона через УЭК">
			<type>list</type>
			<enabled>false</enabled>
			<serviceProviders>
				<serviceProvider name="Sovcombank" visibleName="Совкомбанк">
					<nodes>
						<node id="ift-node1-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>623438</targetProvider>
							<targetService>623438</targetService>
						</node>
                        <node id="ift-node0-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>623438</targetProvider>
							<targetService>623438</targetService>
						</node>
						<node id="ift-node2-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>623438</targetProvider>
							<targetService>623438</targetService>
						</node>
						<node id="mobile.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>688849</targetProvider>
							<targetService>688849</targetService>
						</node>
 						<node id="greenfield1.online.sberbank.ru">
							<targetBilling>284</targetBilling>
							<targetProvider>550478249</targetProvider>
							<targetService>550478249</targetService>
						</node>
 						<node id="greenfield2.online.sberbank.ru">
							<targetBilling>284</targetBilling>
							<targetProvider>500439915</targetProvider>
							<targetService>500439915</targetService>
						</node>
						<node id="node1.online.sberbank.ru">
							<targetBilling>284</targetBilling>
							<targetProvider>629175</targetProvider>
							<targetService>629175</targetService>
						</node>
						<node id="node2.online.sberbank.ru">
							<targetBilling>284</targetBilling>
							<targetProvider>500446239</targetProvider>
							<targetService>500446239</targetService>
						</node>
						<node id="node3.online.sberbank.ru">
							<targetBilling>284</targetBilling>
							<targetProvider>500445546</targetProvider>
							<targetService>500445546</targetService>
						</node>
						<node id="node4.online.sberbank.ru">
							<targetBilling>284</targetBilling>
							<targetProvider>500439915</targetProvider>
							<targetService>500439915</targetService>
						</node>
					</nodes>
				</serviceProvider>
			</serviceProviders>
		</param>
        <param name="P2PTransferByPhoneToOtherBankGroupLayout" description="Группировка пунктов меню (банков) по секциям">
          <type>setting</type>
          <enabled>falsee</enabled>
		</param>
        <param name="P2PExternalBankTransfer2" description="Перевод в другой банк по номеру мобильного телефона">
        	<type>setting</type>
        	<enabled>true</enabled>
          	<historyIcons>true</historyIcons>
            <receiverFromAddressBook>true</receiverFromAddressBook>
		    <stepBackFromConfirmationScreen>true</stepBackFromConfirmationScreen>
          <smartSearchTelNumberBank>true</smartSearchTelNumberBank>
          <smartFind>true</smartFind>
		  <smartFindServices>
			<service serviceId="344:688468:688468:mobile.sberbank.ru" bankId="94578003583:94578005317:344" name="Tinkoff"/>
            <service serviceId="344:689030:689030:mobile.sberbank.ru" bankId="94578003583:94578005317:344" name="Tinkoff"/>
            
            <service serviceId="344:623368:623368:ift-node1-mp.testonline.sberbank.ru" bankId="94578003583:94578005317:344" name="Tinkoff"/>
            <service serviceId="344:623058:623058:ift-node2-mp.testonline.sberbank.ru" bankId="94578003583:94578005317:344" name="Tinkoff"/>
            <service serviceId="284:550478249:550478249:greenfield1.online.sberbank.ru" bankId="94578003583:94578005317:284" name="Tinkoff"/>
            <service serviceId="284:629175:629175:node1.online.sberbank.ru" bankId="94578003583:94578005317:284" name="Tinkoff"/>
            <service serviceId="284:500446239:500446239:node2.online.sberbank.ru" bankId="94578003583:94578005317:284" name="Tinkoff"/>
            <service serviceId="284:500445546:500445546:node3.online.sberbank.ru" bankId="94578003583:94578005317:284" name="Tinkoff"/>
            <service serviceId="284:500439915:500439915:node4.online.sberbank.ru" bankId="94578003583:94578005317:284" name="Tinkoff"/>
           
            <service serviceId="344:1143177:1143177:ift-node1-mp.testonline.sberbank.ru" bankId="95473683409:95473812554:344" name="SovcomBank"/>
            <service serviceId="344:623281:623281:ift-node2-mp.testonline.sberbank.ru" bankId="95473683409:95473812554:344" name="SovcomBank"/>
            <service serviceId="344:688849:688849:mobile.sberbank.ru" bankId="95473683409:95473812554:344" name="SovcomBank"/>
            <service serviceId="344:550478249:550478249:greenfield1.online.sberbank.ru" bankId="95473683409:95473812554:344" name="SovcomBank"/>
            <service serviceId="344:500439915:500439915:greenfield2.online.sberbank.ru" bankId="95473683409:95473812554:344" name="SovcomBank"/>            
		  </smartFindServices>
          <forkPageHint>В Тинькофф банк, Совкомбанк, СДМ Банк</forkPageHint>
		</param>
      	<param name="UsePushAutoDisable" description="активация алгоритма автоотключения push">
          <type>setting</type>
          <enabled>true</enabled>
		</param>
		<param name="brokerage_8_12" description="Брокерское обслуживание">
			<enabled>true</enabled>
			<replenishAccountEnabled>true</replenishAccountEnabled>
			<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
            <createDocApplicationEnabled>true</createDocApplicationEnabled>
            <brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
          	<brokerageProductsAvailableInFinance>true</brokerageProductsAvailableInFinance>
            <brokerageFxWarningEnabled>true</brokerageFxWarningEnabled>
			<nodes>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение Брокерского Счёта</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S133717540667A133717540630)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S133717540667A133717540638)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S133717540667A133717540630)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S133717540667A133717540638)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S133717540667A133717540630)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S133717540667A133717540638)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
     			<node id="10.21.152.7">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S133717540667A133717540630)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S133717540667A133717540638)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                  	<brokerageReplenishmentSelectionMarkets>true</brokerageReplenishmentSelectionMarkets>
				</node>
				<node id="greenfield1.online.sberbank.ru">
                    <enabled>true</enabled>
                    <replenishAccountEnabled>true</replenishAccountEnabled>
                    <replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
                    <replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
                    <replenishAccountAgreementFieldCode>field(S226884898113A226884895980)</replenishAccountAgreementFieldCode>
                    <replenishAccountMarketFieldCode>field(S226884898113A226884895336)</replenishAccountMarketFieldCode>
                    <createDocApplicationEnabled>true</createDocApplicationEnabled>
                    <brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
                    <brokerageProductsAvailableInFinance>true</brokerageProductsAvailableInFinance>
                </node>
			</nodes>
			<markets>
				<market id="0">
					<enabled>true</enabled>
				</market>
				<market id="1">
					<enabled>true</enabled>
				</market>
				<market id="2">
					<enabled>false</enabled>
				</market>
			</markets>
			<brokerageEribMarketsMap>
    			<eribMarket name="Фондовый рынок">
        			<id>0</id>
    			</eribMarket>
    			<eribMarket name="ФБ ММВБ">
        			<id>0</id>
    			</eribMarket>
    			<eribMarket name="ФР ММВБ">
        			<id>0</id>
    			</eribMarket>
    			<eribMarket name="ФР">
        			<id>0</id>
    			</eribMarket>
    			<eribMarket name="Фондовый">
        			<id>0</id>
    			</eribMarket>
    			<eribMarket name="fond">
        			<id>0</id>
    			</eribMarket>
    			<eribMarket name="ФОРТС">
        			<id>1</id>
    			</eribMarket>
    			<eribMarket name="Срочный рынок">
        			<id>1</id>
    			</eribMarket>
    			<eribMarket name="Срочный">
        			<id>1</id>
    			</eribMarket>
    			<eribMarket name="СР">
        			<id>1</id>
    			</eribMarket>
    			<eribMarket name="forts">
        			<id>1</id>
    			</eribMarket>
    			<eribMarket name="Внебиржевой">
        			<id>2</id>
    			</eribMarket>
    			<eribMarket name="Внебиржевой рынок">
        			<id>2</id>
    			</eribMarket>
    			<eribMarket name="ОТС">
        			<id>2</id>
    			</eribMarket>
    			<eribMarket name="Рынок ОТС">
        			<id>2</id>
    			</eribMarket>
    			<eribMarket name="ОТС рынок">
        			<id>2</id>
    			</eribMarket>    
    			<eribMarket name="otc">
        			<id>2</id>
    			</eribMarket>
    			<eribMarket name="Валютный рынок">
        			<id>3</id>
    			</eribMarket>
    			<eribMarket name="Валютный">
        			<id>3</id>
    			</eribMarket>
    			<eribMarket name="ВР">
        			<id>3</id>
    			</eribMarket>
    			<eribMarket name="fx">
        			<id>3</id>
    			</eribMarket>
			</brokerageEribMarketsMap>          
		</param>
	  	<param name="paymentTransactionsEducationEnabled" description="раздел Образование в платежах">
	      <type>service</type>
	      <enabled>true</enabled>
      </param>
		<param name="brokerage" description="Брокерское обслуживание">
			<enabled>true</enabled>
			<replenishAccountEnabled>true</replenishAccountEnabled>
			<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
			<nodes>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>
     			<node id="10.21.152.7">
					<enabled>true</enabled>
					<replenishAccountEnabled>true</replenishAccountEnabled>
					<replenishAccountInMarginCallEnabled>true</replenishAccountInMarginCallEnabled>
					<replenishAccountSearchString>Пополнение брокерского счета</replenishAccountSearchString>
					<replenishAccountAgreementFieldCode>field(S85396525721A85396525552)</replenishAccountAgreementFieldCode>
					<replenishAccountMarketFieldCode>field(S85396525721A85396525571)</replenishAccountMarketFieldCode>
					<createDocApplicationEnabled>true</createDocApplicationEnabled>
            		<brokerageHelpPhoneNumber>900</brokerageHelpPhoneNumber>
				</node>

			</nodes>
			<markets>
				<market id="0">
					<enabled>true</enabled>
				</market>
				<market id="1">
					<enabled>true</enabled>
				</market>
				<market id="2">
					<enabled>false</enabled>
				</market>
			</markets>
		</param>
	  	<param name="paymentTransactionsEducationEnabled" description="раздел Образование в платежах">
	      <type>service</type>
	      <enabled>true</enabled>
      </param>
      <param name="TxPushSuggestion" description="">
          <type>setting</type>
          <enabled>true</enabled>
          <periodInDays>1</periodInDays>
          <number>5</number>
      </param>
      <param name="nodeDoNotShowPushTutorialForApiLevels" description="">
        <type>list</type>
            <nodes>
               <node id="greenfield1.online.sberbank.ru">
                   <enabled>true</enabled>
               </node>
            	<node id="greenfield2.online.sberbank.ru">
                   <enabled>true</enabled>
               </node>
               <node id="mobile.sberbank.ru">
                   <enabled>true</enabled>
               </node>
               <node id="ift-node1.testonline.sberbank.ru">
                   <enabled>true</enabled>
               </node>
               <node id="ift-node2.testonline.sberbank.ru">
                   <enabled>true</enabled>
               </node>
               <node id="ift-node1-mp.testonline.sberbank.ru">
                   <enabled>true</enabled>
               </node>
               <node id="ift-node2-mp.testonline.sberbank.ru">
                   <enabled>true</enabled>
               </node>
            </nodes>
      </param>
      <param name="CardPushEnabled" description="">
        <type>setting</type>
        <enabled>true</enabled>
      </param>
      <param name="DDAPermissions" description="Консолидированные включатели функционала Data Driven App">
			<type>list</type>
    		<enabled>true</enabled>
        	<DDPSbermetricaServiceEnabled>true</DDPSbermetricaServiceEnabled>
			<DDASmartSearchFeedBackEnabled>true</DDASmartSearchFeedBackEnabled>
        	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
            <DDPCardPersHideEnabled>true</DDPCardPersHideEnabled>
        	<DDPAnalyticsDownloadedWithHashEnabled>true</DDPAnalyticsDownloadedWithHashEnabled>
        	<DDPAnalyticsCardsClickWithHashEnabled>true</DDPAnalyticsCardsClickWithHashEnabled>
    		<nodes>
        		<node id="node0.online.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<DDPCardPersSortEnabled>false</DDPCardPersSortEnabled>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                    <SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                </node>
        		<node id="node1.online.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                  	<MessengerSmartSearch>true</MessengerSmartSearch>
                    <SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                  	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
        		</node>
        		<node id="node2.online.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                  	<MessengerSmartSearch>true</MessengerSmartSearch>
                    <SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                  	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
        		</node>
        		<node id="node3.online.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                  	<MessengerSmartSearch>true</MessengerSmartSearch>
                    <SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                    <DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
        		</node>
        		<node id="greenfield1.online.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
                    <DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPProvidersRelevantSearchEnabled>true</DDPProvidersRelevantSearchEnabled>
                  	<DDPSearchExamples>true</DDPSearchExamples>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                  	<MessengerSmartSearch>false</MessengerSmartSearch>
                    <DDPCardPersHideEnabled>true</DDPCardPersHideEnabled>
                  	<CustomShowAllScreenForHistory>true</CustomShowAllScreenForHistory>
                	<SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                  	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
        		</node>
        		<node id="greenfield2.online.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPProvidersRelevantSearchEnabled>true</DDPProvidersRelevantSearchEnabled>
                  	<DDPSearchExamples>true</DDPSearchExamples>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                  	<MessengerSmartSearch>true</MessengerSmartSearch>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
        		</node>
                <node id="194.186.207.23">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                    <SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
              </node>
              <node id="mobile.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                	<DDPCardPersHideEnabled>true</DDPCardPersHideEnabled>
                	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                	<SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
                	<MessengerSmartSearch>true</MessengerSmartSearch>
                	<RetryRequest>2</RetryRequest>
        	</node>
          	  <node id="ift-node1.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
            </node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                    <CustomShowAllScreenForHistory>true</CustomShowAllScreenForHistory>
              </node>
              <node id="ift-node5-mp.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
                	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                    <CustomShowAllScreenForHistory>true</CustomShowAllScreenForHistory>
              </node>
              <node id="ift-node7-mp.testonline.sberbank.ru">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
            </node>
            <node id="msv-node2.testonline.sberbank.ru">
            		<SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>  
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
              </node>
            <node id="ift-node5.testonline.sberbank.ru">  
            		<SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
              </node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
                	<SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
                  	<DDPCardPersSortEnabled>true</DDPCardPersSortEnabled>
              		<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
              </node>
              <node id="10.21.152.7">
      	    	    <SmartSearch>true</SmartSearch>
        	    	<NBAA>true</NBAA>
                    <SearchHistory>true</SearchHistory>
            		<DepthNBAA>60</DepthNBAA>
         		    <MonthAmountNBAA>3</MonthAmountNBAA>
                    <SearchForHistoryWithListDo>true</SearchForHistoryWithListDo>
					<HistoryPageCount>3</HistoryPageCount>
					<RequestDelay>400</RequestDelay>
					<NBAAForHistoryDisabled>true</NBAAForHistoryDisabled>
					<NBAAForPaymentsDisabled>true</NBAAForPaymentsDisabled>
					<MainNotification>true</MainNotification>
					<DDPSmartNbaaEnabled>true</DDPSmartNbaaEnabled>
					<DDPContactsWeightsEnabled>true</DDPContactsWeightsEnabled>
					<DDPNBAARepeatEnabled>true</DDPNBAARepeatEnabled>
                    <DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
					<NLPEnabled>true</NLPEnabled>
                    <ApplePayAdd>false</ApplePayAdd>
                    <BlockCardAdd>true</BlockCardAdd>
                    <CurrencyCardBankDetail>true</CurrencyCardBankDetail>
                  	<DDPProvidersRelevantSearchEnabled>true</DDPProvidersRelevantSearchEnabled>
                  	<DDPSearchExamples>true</DDPSearchExamples>
                  	<DDPCardPersSortEnabled_v2>true</DDPCardPersSortEnabled_v2>
                  	<BatchLength>10</BatchLength>
					<BatchSendingInterval>10</BatchSendingInterval>
                  	<MessengerSmartSearch>false</MessengerSmartSearch>
                    <DDPCardPersHideEnabled>true</DDPCardPersHideEnabled>
                  	<CustomShowAllScreenForHistory>true</CustomShowAllScreenForHistory>
                	<SmartSearchWidgetsPayment>true</SmartSearchWidgetsPayment>
                  	<DDPBusinessChatsEnabled>true</DDPBusinessChatsEnabled>
        		</node>
    		</nodes>
		</param>
    	<param name="InsuranceProducts" description="Продажа страховых продуктов">
          <type>list</type>
          <nodes>
            <node id="greenfield1.online.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="194.186.207.23">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="mobile.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="node0.online.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="node1.online.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="node2.online.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="node3.online.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="ift-node1.testonline.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
			  <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="ift-node7-mp.testonline.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="10.21.152.7">
              <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
            <node id="msv-node2.testonline.sberbank.ru">
               <InsuranceProductsEnabled>true</InsuranceProductsEnabled>
            </node>
          </nodes>
        </param>
      	<param name="providerUFSPaymentsEnabled" description="Платежи в МП на ЕФС">
          <type>setting</type>
          <enabled>true</enabled>
      	</param>
        <param name="PersonalDataProfile" description="Редактирование/добавление персональных данных клиента">
            <type>list</type>
            <enabled>true</enabled>
            <nodes>
              <node id="mobile.sberbank.ru">
                    <enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                    <EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
              </node>
              <node id="psinode2.testonline.sberbank.ru">
                    <enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>false</PhoneNumberSMSConfirmationProfile>
                    <EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
              </node>
              <node id="psinode1.testonline.sberbank.ru">
                    <enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>false</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>false</PhoneNumberSMSConfirmationProfile>
             	    <EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
              </node>
              <node id="194.186.207.23">
                    <enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
               		<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
			  </node>
              <node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>true</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                    <HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                    <CashingPersonalDataProfile>false</CashingPersonalDataProfile>
             	    <EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
			  </node>
              <node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
               		<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                  	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                  	<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                  	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                  	<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
				</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                  	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                  	<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                  	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                  	<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
				</node>
              <node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
					<PassportProfile>false</PassportProfile>
					<EmailProfile>true</EmailProfile>
					<PhoneNumberProfile>true</PhoneNumberProfile>
					<DriversLicenseProfile>true</DriversLicenseProfile>
					<STSProfile>true</STSProfile>
					<InnProfile>true</InnProfile>
					<SnilsProfile>true</SnilsProfile>
                  	<HistoryOperationProfile>true</HistoryOperationProfile>
                    <EmailEditProfile>true</EmailEditProfile>
                    <PhoneNumberEditProfile>true</PhoneNumberEditProfile>
                    <SnilsEditProfile>false</SnilsEditProfile>
                    <InnEditProfile>false</InnEditProfile>
                    <PhoneNumberSMSConfirmationProfile>true</PhoneNumberSMSConfirmationProfile>
                  	<EmailDoubleAddProfile>true</EmailDoubleAddProfile>
                    <PhoneNumberDoubleAddProfile>true</PhoneNumberDoubleAddProfile>
				</node>
             </nodes>
        </param>
		<param name="SberbankIDMerchantIcon" description="Иконка потребителя">
			<type>source</type>
			<link>/SBERBANKID/icons/client_id.png</link>
		</param>
        <param name="HistoryOperation" description="Вкладка История. Блоки работают по логическому ИЛИ">
        	<newFiltersInHistory>true</newFiltersInHistory>
		<nodes>
			<node id="node0.online.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
                <extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="node1.online.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
            <extendedFiltersInHistory>true</extendedFiltersInHistory>
            </node>
			<node id="node2.online.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
                <logotypesInOperationDetails>true</logotypesInOperationDetails>
                <mapInOperationDetails>true</mapInOperationDetails>
                <replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
                <bonusInHistory>true</bonusInHistory>
                <creditCardCommissionInHistory>true</creditCardCommissionInHistory>
                <showExtEpsPayment>true</showExtEpsPayment>
                <extEpsOperationRepeat>true</extEpsOperationRepeat>
            <extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="node3.online.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
               	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
            <extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="greenfield1.online.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>false</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="greenfield2.online.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
			    <externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="mobile.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
             	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
             	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
              	<newFiltersInHistory>true</newFiltersInHistory>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="ift-node1.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
				<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
                <mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="ift-node2.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
        	  	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
				<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
                <mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>           
			</node>
			<node id="ift-node1-mp.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
    	      	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
    	      	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
              	<mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			<node id="ift-node2-mp.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
      	    	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
                <mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>true</extEpsPaymentOperation>
            	<hideExtEpsOperationRepeat>true</hideExtEpsOperationRepeat>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
              	<bonusInHistory>true</bonusInHistory>
              	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
          <node id="ift-node5-mp.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
      	    	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
                <mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
            	<extEpsPaymentsForm>true</extEpsPaymentsForm>
            	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
            	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
            	<bonusInHistory>true</bonusInHistory>
            	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
          <node id="ift-node7-mp.testonline.sberbank.ru">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
      	    	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
                <smartSearchFromHistory>true</smartSearchFromHistory>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
                <mapInOperationDetails>true</mapInOperationDetails>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
            	<extEpsPaymentsForm>true</extEpsPaymentsForm>
            	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
            	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
            	<bonusInHistory>true</bonusInHistory>
            	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>			
          <node id="10.21.152.7">
                <paymentHistoryOpenAnimation>true</paymentHistoryOpenAnimation>
				<externalOperationForm>true</externalOperationForm>
				<newOperationsHistoryList>true</newOperationsHistoryList>
	          	<hideDaySum>false</hideDaySum>
                <tagAll>true</tagAll>
                <additionalOperationForm>true</additionalOperationForm>
                <logotypes>true</logotypes>
                <routerForUFS>true</routerForUFS>
                <replaceInvoicesToHistory>true</replaceInvoicesToHistory>
                <smartSearchFromHistory>true</smartSearchFromHistory>
                <receiveOperationsByTag>true</receiveOperationsByTag>
                <replaceInvoicesToHistoryOnAccount>true</replaceInvoicesToHistoryOnAccount>
                <refactoredOperationDetails>true</refactoredOperationDetails>
              	<referenceOnOperation>true</referenceOnOperation>
              	<logotypesInOperationDetails>true</logotypesInOperationDetails>
              	<mapInOperationDetails>true</mapInOperationDetails>
            	<arrestAndPunishmentOperations>true</arrestAndPunishmentOperations>
              	<advertisementInHistoryList>true</advertisementInHistoryList>
              	<extEpsPaymentOperation>false</extEpsPaymentOperation>
              	<extEpsPaymentsForm>true</extEpsPaymentsForm>
              	<replaceInvoicesToHistoryInTargets>true</replaceInvoicesToHistoryInTargets>
              	<showExtEpsPayment>true</showExtEpsPayment>
              	<extEpsOperationRepeat>true</extEpsOperationRepeat>
           		<bonusInHistory>true</bonusInHistory>
            	<creditCardCommissionInHistory>true</creditCardCommissionInHistory>
            	<extendedFiltersInHistory>true</extendedFiltersInHistory>
			</node>
			</nodes>
		</param>
		<param name="DelayCuteCheck" description="время ожидания ответа с обогащённым контентом">
    		<type>setting</type>
    		<enabled>true</enabled>
    		<delay>20</delay>
		</param>
		<param name="TPNDataEnrichment" description="Возможность обогащения данных для ТПУ на разрешенных нодах">
    		<type>setting</type>
   			<enabled>true</enabled>
		</param>
		<param name="NodeTPNDataEnrichment" description="Возможность обогащения данных для ТПУ на разных нодах">
			<type>list</type>
			<nodes>
				<node id="greenfield0.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
              	<node id="greenfield1.online.sberbank.ru">
                  <enabled>true</enabled>
                </node>
				<node id="psinode1.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
			</nodes>
		</param>
      	<param name="notificationStripeHistory" description="">
            <type>setting</type>
            <enabled>true</enabled>
            <nodes>
                <node id="node0.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
              	<node id="greenfield0.online.sberbank.ru">
                  <enabled>true</enabled>
                </node>
              	<node id="greenfield1.online.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="psinode1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="mobile.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="194.186.207.23">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
             </nodes>
        </param>
      	<param name="notificationStripeFilter" description="">
            <type>setting</type>
            <enabled>true</enabled>
            <nodes>
                <node id="node0.online.sberbank.ru">
                    <enabled>true</enabled>
                </node>
              	<node id="greenfield0.online.sberbank.ru">
                  <enabled>true</enabled>
                </node>
              	<node id="greenfield1.online.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="psinode1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="mobile.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="194.186.207.23">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
             </nodes>
        </param>
		<param name="biometryAgreement" description="">
			<type>list</type>
			<enabled>true</enabled>
          	<showTutorial>true</showTutorial>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
				</node>
                <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
                <node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
			</nodes>
		</param>
		<param name="NativeAppsCheck" description="">
			<type>list</type>
			<enabled>true</enabled>
          	<enabledV2>true</enabledV2>
          	<usingSilentPush>true</usingSilentPush>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
                <node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
                <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
              	<node id="psinode2.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
             	 <node id="psinode1.testonline.sberbank.ru">
					<enabled>true</enabled>
                   	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
               <node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                 	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
          			<usingSilentPush>true</usingSilentPush>
				</node>
			</nodes>
		</param>
		<param name="BiometricsTemplateCreate" description="">
			<type>list</type>
			<enabled>true</enabled>
          	<enabledV2>true</enabledV2>
          	<enabledV3>true</enabledV3>
          	<originalBestshotEnabled>true</originalBestshotEnabled>
          	<activeTemplateCreation>true</activeTemplateCreation>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>false</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
                <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>false</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledV2>true</enabledV2>
                  	<enabledV3>true</enabledV3>
          			<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<activeTemplateCreation>true</activeTemplateCreation>
				</node>
              <node id="greenfield1.online.sberbank.ru">
					<enabled>false</enabled>
                  	<enabledV2>false</enabledV2>
                    <enabledV3>true</enabledV3>
                  	<activeTemplateCreation>true</activeTemplateCreation>
                	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
			</nodes>
		</param>
		<param name="ConfirmationBiometricsVoice" description="">
			<type>list</type>
			<enabled>true</enabled>
          	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          	<enabledInMessenger>true</enabledInMessenger>
          	<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          	<enabledInPaymentsV2>true</enabledInPaymentsV2>
          	<lightSchemeForMessenger>true</lightSchemeForMessenger>
          	<originalBestshotEnabled>true</originalBestshotEnabled>
          	<personalLimitEnabled>true</personalLimitEnabled>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
                    <enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ruu">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
                <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>false</originalBestshotEnabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
                  	<personalLimitEnabled>true</personalLimitEnabled>
				</node>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledInP2PTransfer>true</enabledInP2PTransfer>
          			<enabledInMessenger>true</enabledInMessenger>
          			<enabledInInternalPaymentsV2>true</enabledInInternalPaymentsV2>
          			<enabledInPaymentsV2>true</enabledInPaymentsV2>
                  	<lightSchemeForMessenger>true</lightSchemeForMessenger>
                  	<originalBestshotEnabled>true</originalBestshotEnabled>
				</node>
			</nodes>
		</param>
		<param name="biometryAgreementStartPage" description="">
			<type>list</type>
			<enabled>true</enabled>
          	<enabledUFS7>true</enabledUFS7>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
                 	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
                <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
              	<node id="ift-node0-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
                  	<enabledUFS7>true</enabledUFS7>
				</node>
			</nodes>
		</param>
		<param name="BiometricsLivenessChecks" description="Настройки проверок на человечность в биометрических процессах">
			<enabled>true</enabled>
            <processes>
                <process name="ConfirmationBiometrics">
                    <enabled>true</enabled>
                    <livenessType>BLINK</livenessType>	
                </process>
                <process name="BiometricsTemplateCreate">
                    <enabled>true</enabled>
                    <livenessType>HEADMOVE|BLINK</livenessType>	
                </process>
            </processes>
		</param>
      	<param name="UFSWidgetConfirmationBiometrics" description="">
			<type>list</type>
			<enabled>true</enabled>
			<nodes>
				<node id="node0.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node1.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node2.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="node3.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="greenfield1.online.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="194.186.207.23">
					<enabled>true</enabled>
				</node>
				<node id="mobile.sberbank.ru">
					<enabled>true</enabled>
				</node>
                <node id="mobile4.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
              	<node id="ift-node7-mp.testonline.sberbank.ru">
					<enabled>true</enabled>
				</node>
            </nodes>
		</param>
		<param name="LoanNavigationScreenEnabled" description="Разводной экран для кредитных продуктов">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="PushHistoryFastScroll" description="">
            <type>setting</type>
            <enabled>true</enabled>
        </param>
        <param name="SBOLBage" description="">
            <type>setting</type>
            <enabled>true</enabled>
            <nodes>
                <node id="mobile.sberbank.ru">
                    <enabled>true</enabled>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                </node>
        		<node id="ift-node2.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
        		<node id="ift-node1-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
        		<node id="ift-node2-mp.testonline.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
        		<node id="greenfield1.online.sberbank.ru">
            		<enabled>true</enabled>
        		</node>
            </nodes>
            <levels>
                <level id="showAnimatedBagePostLoginHistory">
                    <enabled>true</enabled>
                </level>
                <level id="showBagePostLoginHistory">
                    <enabled>true</enabled>
                </level>
                <level id="showBagePreLogin">
                    <enabled>true</enabled>
                </level>
                <level id="showBageOnAppIcon">
                    <enabled>true</enabled>
                </level>
              	<level id="showBadgePostLoginTabbar">
                    <enabled>true</enabled>
                </level>
              	<level id="showBadgePostLoginNavBar">
                    <enabled>true</enabled>
                </level>
            </levels>
        </param>
    	<param name="DebitCardNegativeBalanceButton" description="Вынесение подсказки по отрицательном балансе в отдельный экран">
        <type>service</type>
        <enabled>false</enabled>
        <nodes>
            <node id="node0.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="mobile.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node3.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node7-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="194.186.207.23">
                <enabled>true</enabled>
            </node>
        </nodes>
    	</param>
    
		<param name="MAppDebitCardNegativeBalance" description="Почему минус на дебетовой карте">
     		<type>service</type>
     		<enabled>true</enabled>  			
        </param>
    
		<param name="CurrenciesAndMetalsFlags" description="Вылюта и металлические счета">
					<type>list</type>
					<enabled>true</enabled>
					<nodes>
						<!-- Параметр imaOfficeChoiceDisabled отключение выбора ВСП при открытии ОМС. Применяется с версии 9.9. -->
						<node id="mobile.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="node0.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="node1.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="node2.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="node3.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="node4.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="greenfield1.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="greenfield2.online.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="ift-node1-mp.testonline.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="ift-node2-mp.testonline.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="ift-node3-mp.testonline.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="ift-node4-mp.testonline.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="psinode1.testonline.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
						<node id="psinode2.testonline.sberbank.ru">
							<imaOfficeChoiceDisabled>true</imaOfficeChoiceDisabled>
						</node>
					</nodes>
				</param>

				<param name="DepositsFlags" description="Вклады">
					<type>list</type>
					<enabled>true</enabled>
					<minorsLimit>30500</minorsLimit>
					<appAdditionalPercentage>0.05</appAdditionalPercentage>
					<!--Смотрим на параметр depCloseAlert с версии 9.9-->
					<depCloseAlert>false</depCloseAlert>
					<!-- Настройка предупреждающих сообщений при разнице валют -->
					<diffCurrencyTexts>
						<diffCurrencyText id="Normal">
							<DCWarningTitle>Не теряйте деньги на&#xA0;конвертации</DCWarningTitle>
							<DCWarningText>Валюты вклада и выбранного счёта не&#xA0;совпадают, поэтому перевод пройдёт по&#xA0;текущему курсу обмена.&#10;Чтобы не&#xA0;терять деньги, выберите счёт в&#xA0;валюте вклада.</DCWarningText>
							<DCWarningOkButton>ВСЁ РАВНО ПЕРЕВЕСТИ</DCWarningOkButton>
							<DCWarningCancelButton>ВЫБРАТЬ ДРУГОЙ СЧЁТ</DCWarningCancelButton>
						</diffCurrencyText>
						<diffCurrencyText id="Pref">
							<DCWarningTitle>Не теряйте деньги на&#xA0;конвертации</DCWarningTitle>
							<DCWarningText>Валюты вклада и выбранного счёта не&#xA0;совпадают, поэтому перевод пройдёт по&#xA0;льготному курсу обмена.&#10;Чтобы не&#xA0;терять деньги, выберите счёт в&#xA0;валюте вклада.</DCWarningText>
							<DCWarningOkButton>ВСЁ РАВНО ПЕРЕВЕСТИ</DCWarningOkButton>
							<DCWarningCancelButton>ВЫБРАТЬ ДРУГОЙ СЧЁТ</DCWarningCancelButton>
						</diffCurrencyText>
					</diffCurrencyTexts>

					<maxBalance>
						<multiplier>10</multiplier>
						<limit currency="RUB">1000000</limit>
						<limit currency="USD">50000</limit>
						<limit currency="EUR">50000</limit>
					</maxBalance>
					
					<nodes>
						<!--Смотрим на параметр amountPickerShowHintPopoverNew с версии 9.6-->
						<!--Смотрим на параметр diffCurrencyWarning с версии 9.8-->
						<node id="mobile.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="node0.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="node1.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="node2.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="node3.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="node4.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="greenfield1.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="greenfield2.online.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="ift-node1-mp.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
                        <node id="ift-node0-mp.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="ift-node2-mp.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="ift-node3-mp.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="ift-node4-mp.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="ift-node5-mp.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="psinode1.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
						<node id="psinode2.testonline.sberbank.ru">
							<minorsWarning>true</minorsWarning>
							<autoSelectionForDepositTransferToResource>true</autoSelectionForDepositTransferToResource>
							<amountPickerShowHintPopoverNew>true</amountPickerShowHintPopoverNew>
							<accountOpeningRedesignEnabled>true</accountOpeningRedesignEnabled>
							<diffCurrencyWarning>true</diffCurrencyWarning>
						</node>
					</nodes>
				</param>

      <param name="DepositsSliderMaxValue" description="Изменение правой границы бегунка суммовой градации во вкладах">
           <type>list</type>
           <enabled>true</enabled>
 	 </param>
	<param name="PromoCodeActivation" description="Ввод промо-кодов для вкладов">
		<type>setting</type>
		<enabled>true</enabled>
	</param>
    <param name="customERIBInfantWarning" description="Информирование несовершеннолетних клиентов">
		<type>setting</type>
		<enabled>true</enabled>
	</param>
    <param name="SaveUserSelectionParameters" description="Пакет улучшений клиентского опыта по открытию вкладов">
           <type>list</type>
           <enabled>true</enabled>
       <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
 	 </param>
      <param name="CollapseDepositsOfSameType" description="Оптимизация отображения вкладов, доступных для открытия">
           <type>list</type>
           <enabled>true</enabled>
           <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
 	 </param>
      <param name="CollapseDepositsOfSameTypeWithoutDistinctUnion" description="Изменение отображения Условий вклада при открытии">
           <type>list</type>
           <enabled>true</enabled>
        <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
 	 </param>
      <param name="vspAddress" description="Реквизиты ВСП вклада">
           <type>list</type>
           <enabled>true</enabled>
          <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
 	 </param>
      <param name="depositMaxBalance" description="Отображение максимальной суммы вклада">
           <type>list</type>
           <enabled>true</enabled>
           <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
 	 </param>
      <param name="SmartDepositDatePicker" description="Изменение работы инструмента выбора срока вклада">
           <type>list</type>
           <enabled>true</enabled>
            <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
		 </param>
      <!--Смотрим на параметр AmountPickerShowHintPopover в версии 9.5-->
        <param name="AmountPickerShowHintPopover" description="Облако с подсказкой о том, что большую сумму можно ввести руками">
           <type>list</type>
           <enabled>true</enabled>
           <nodes>
            <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node0.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
             <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
            	<enabled>true</enabled>
          	</node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
               <enabled>true</enabled>
            </node>
           </nodes>
 	 </param>
         <param name="PriorityCardP2PService" description="Установка приоритетной карты для зачисления P2P Переводов по НМТ">
         	<pendingOperationViewEnabled>false</pendingOperationViewEnabled>
           <type>setting</type>
           <enabled>true</enabled>
        </param>
        <param name="PriorityCardP2PServiceTutorial" description="Туториал для приоритетной карты">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
      	<param name="PushPermissions" description="единый стек параметров для push">
			<type>list</type>
            <pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
          	<pushHistoryHeadBatchSize>50</pushHistoryHeadBatchSize>
			<pushHistoryScrollBatchSize>50</pushHistoryScrollBatchSize>
          	<countFbQualityDemonstration>3</countFbQualityDemonstration>
          	<fbQualityPercentEnough>90</fbQualityPercentEnough>
          	<fbEqualCount>false</fbEqualCount>
			<nodes>
                <node id="ift-node0-mp.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
					<pushLogoTypeUsing>true</pushLogoTypeUsing>
					<getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
					<MessagesWithExpired>false</MessagesWithExpired>
					<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
					<NotificationSettingsOwn>true</NotificationSettingsOwn>
					<showNewAttributesInPushContent>true</showNewAttributesInPushContent>
					<showUniversalPushNotification>true</showUniversalPushNotification>
					<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
					<XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                  	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                </node>
				<node id="greenfield0.online.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
                  	<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
					<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
					<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
					<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
                  	<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>false</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                    <importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
              	<node id="greenfield1.online.sberbank.ru">
                  	<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
					<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>                  
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                    <importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                  	<copyAndShareNotification>true</copyAndShareNotification>
                </node>
                <node id="node0.online.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
					<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
					<NotificationSettingsOwn>true</NotificationSettingsOwn>
					<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
					<TurnOffOperationPush>true</TurnOffOperationPush>
					<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
					<showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
					<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>                  	
                  	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
                <node id="node1.online.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
					<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
					<NotificationSettingsOwn>true</NotificationSettingsOwn>
					<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
					<TurnOffOperationPush>true</TurnOffOperationPush>
					<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
					<showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                    <importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
                <node id="node2.online.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
					<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
					<NotificationSettingsOwn>true</NotificationSettingsOwn>
					<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
					<TurnOffOperationPush>true</TurnOffOperationPush>
					<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
					<showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
                <node id="node3.online.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
					<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
					<NotificationSettingsOwn>true</NotificationSettingsOwn>
					<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
					<TurnOffOperationPush>true</TurnOffOperationPush>
					<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
					<showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
                <node id="node4.online.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
					<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
					<NotificationSettingsOwn>true</NotificationSettingsOwn>
					<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
					<TurnOffOperationPush>true</TurnOffOperationPush>
					<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
					<showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
				<node id="psinode1.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
					<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
				<node id="mobile.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                  	<changePhoneAndTariffFromProfileEditor>false</changePhoneAndTariffFromProfileEditor>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>false</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                  	<copyAndShareNotification>true</copyAndShareNotification>
				</node>
				<node id="194.186.207.23">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                  	<changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>	
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
                    <MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <PUSHNotificationsTransactionContentExtension>true</PUSHNotificationsTransactionContentExtension>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                  	<copyAndShareNotification>true</copyAndShareNotification>
				</node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
                  	<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>true</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                  	<copyAndShareNotification>true</copyAndShareNotification>
				</node>
              <node id="ift-node5-mp.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <PUSHNotificationsTransactionContentExtension>true</PUSHNotificationsTransactionContentExtension>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                  	<copyAndShareNotification>true</copyAndShareNotification>
				</node>
              <node id="ift-node7-mp.testonline.sberbank.ru">
					<buttonToPostLogin>true</buttonToPostLogin>
            		<pushHistoryAvailableInTabbarBank>true</pushHistoryAvailableInTabbarBank>
					<MFMSMessageRequestType>2</MFMSMessageRequestType>
                  	<NotificationSettingsOwn>true</NotificationSettingsOwn>
                  	<autoTurnOffOperationPush>true</autoTurnOffOperationPush>
                  	<TurnOffOperationPush>true</TurnOffOperationPush>
                  	<MessagesWithExpired>true</MessagesWithExpired>
                  	<showBestActionsInCuteCheque>true</showBestActionsInCuteCheque>
                    <showNotificationEntryPointTargetTapPrelogin>true</showNotificationEntryPointTargetTapPrelogin>
					<showNotificationEntryPointTargetTapPostlogin>true</showNotificationEntryPointTargetTapPostlogin>
					<newRejectAuthorizeAlert>true</newRejectAuthorizeAlert>
                    <showAlertBeforeTPUDisable>true</showAlertBeforeTPUDisable>
                  	<showUniversalPushNotification>true</showUniversalPushNotification>
                    <getMessageHistoryRequestEnabled>true</getMessageHistoryRequestEnabled>
					<nativePushProcessingEnabled>true</nativePushProcessingEnabled>
                  	<webUrlInUniversalPushNotification>true</webUrlInUniversalPushNotification>
                    <cardNotificationWithSenderNameAndComment>true</cardNotificationWithSenderNameAndComment>
                    <routingFromTransactionPushToMessengerEnabled>true</routingFromTransactionPushToMessengerEnabled>
                  	<pushLogoTypeUsing>true</pushLogoTypeUsing>
                    <UsePushAutoDisable>true</UsePushAutoDisable>
                    <reactivateMainPushNotifications>true</reactivateMainPushNotifications>
                    <hideMainPushNotificationsSwitcher>true</hideMainPushNotificationsSwitcher>
                    <PUSHNotificationsTransactionContentExtension>true</PUSHNotificationsTransactionContentExtension>
                    <XMLHeaderEncodingFix>true</XMLHeaderEncodingFix>
                    <transferTPUSettingsOnNewRegistration>true</transferTPUSettingsOnNewRegistration>
                  	<pushGlobalSearchByKeywords>true</pushGlobalSearchByKeywords>
					<newAlertWhenTPUActivate>true</newAlertWhenTPUActivate>
                    <reactivateMainPushNotifications2>true</reactivateMainPushNotifications2>
                  	<transactionNewTutorialAvailable>true</transactionNewTutorialAvailable>
                  	<forcedHistoryQuery>true</forcedHistoryQuery>
					<forcedHistoryQueryIfNoHistory>true</forcedHistoryQueryIfNoHistory>
                    <NewNotificationsListFilter>true</NewNotificationsListFilter>
                    <tutorialAboutAutomaticTransferTPUSettings>true</tutorialAboutAutomaticTransferTPUSettings>
                    <NewNotificationsList>true</NewNotificationsList>
                    <NewNotificationsListHistory>true</NewNotificationsListHistory>
                    <NewNotificationsListSearch>true</NewNotificationsListSearch>
                  	<newPushAutoTurn>true</newPushAutoTurn>
                    <enableDeletePushMessage>true</enableDeletePushMessage>
                  	<TransferOrTurnOn2>true</TransferOrTurnOn2>
            		<TransferMethod>manual</TransferMethod>
            		<TransferMethodAA>manual</TransferMethodAA>
            		<TurnOnMethodNC>manual</TurnOnMethodNC>
            		<TransferMethodHA>manual</TransferMethodHA>
                  	<TransferMethodTC>true</TransferMethodTC>
                	<importantPushOnMainScreen>true</importantPushOnMainScreen>
                    <NotificationServiceExtensionDisabled>false</NotificationServiceExtensionDisabled>                  
                    <fastBalanceAvailable>true</fastBalanceAvailable>
                  	<copyAndShareNotification>true</copyAndShareNotification>
				</node>
			</nodes>
          	<bestActions>
              	<actions>
					<bestActions name="Перевод клиенту Сбербанка" link="sberbankonline://payments/p2p-by-card-number"/>
					<bestActions name="ЖКХ и домашний телефон" link="sberbankonline://payments/jkh"/>
					<bestActions name="Мобильная связь" link="sberbankonline://payments/mobile-phone"/>
                </actions>
                <actions96>
                	<bestActions name="Перевод клиенту Сбербанка" link="sberbankonline://payments/p2p-by-phone-number"/>
                	<bestActions name="ЖКХ и домашний телефон" link="sberbankonline://payments/jkh"/>
                	<bestActions name="Мобильная связь" link="sberbankonline://payments/mobile-phone"/>
                </actions96>
              	<operationAmount>1000</operationAmount>
            </bestActions>
            <NotificationsListFilters>
              	<NotificationsListFilter>
                  <identifier>all</identifier>
                  <name>Все</name>
                  <type>default</type>
                </NotificationsListFilter>
              	<NotificationsListFilter>
                  <identifier>payment_out</identifier>
                  <name>Списания</name>
                  <type>transaction</type>
                  <operationTypes>- ! ( [ { } 0 1 2 3 4 5 A2 A3 A4 A5 A6 A7 A8 A9 AA AB AC AD AE AU D2 D6 F G K M O R T</operationTypes>
        		</NotificationsListFilter>
              	<NotificationsListFilter>
                  <identifier>payment_in</identifier>
                  <name>Зачисления</name>
                  <type>transaction</type>
                  <operationTypes>* # @ &amp; ) ] 6 7 A A0 A1 B C D D1 D3 D7 E I L N P Q R2 R3 R4 R5 R6 R7 R8 R9 RA RB RC RD RE RU S U</operationTypes>
        		</NotificationsListFilter>
              	<NotificationsListFilter>
                  <identifier>cash</identifier>
                  <name>Наличные</name>
                  <type>transaction</type>
                  <operationTypes>2 D2 B D5 4 D D3</operationTypes>
        		</NotificationsListFilter>
              	<NotificationsListFilter>
                  <identifier>p2p</identifier>
                  <name>Переводы</name>
                  <type>transaction</type>
                  <operationTypes>! * A0 A1 A9 AT AV M N R0 R1 R9 RB RT RV AG AH RG RH</operationTypes>
        		</NotificationsListFilter>
              <NotificationsListFilter>
                  <identifier>marketing</identifier>
                  <name>Маркетинговые</name>
                  <type>default</type>
                  <pushTypes>101 102</pushTypes>
        		</NotificationsListFilter>             
            </NotificationsListFilters>
		</param>
      	<param name="MAppNewBlockCardProcess" description="Обновленный процесс блокировки карт">
                  <type>service</type>
                  <enabled>true</enabled>
           <nodes>
              <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="mobile.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node0-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="194.186.207.23">
            <enabled>true</enabled>
          </node>
        </nodes>
	  </param>
    
      <param name="PlasticCardLifeCycleAllMessages" description="Информационные сообщения по жизненному циклу карт">
        <type>service</type>
        <enabled>true</enabled>
      </param> 
    
      <param name="InternalPaymentForCreditCardDebts_v3" description="Подстановка суммм задолженностей по кредитной карте при переводе между своими счетами">
        <type>service</type>
           <enabled>true</enabled>
        <nodes>
          <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node4.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node5.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="mobile.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="194.186.207.23">
            <enabled>true</enabled>
          </node>
        </nodes>
      </param>
      <param name="InternalPaymentForCreditCardDebts_v2" description="Подстановка суммм задолженностей по кредитной карте при переводе между своими счетами">
        <type>service</type>
           <enabled>true</enabled>
        <nodes>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
        </nodes>
      </param>
      <param name="InternalPaymentForCreditCardDebts_v3" description="Подстановка суммм задолженностей по кредитной карте при переводе между своими счетами">
        <type>service</type>
           <enabled>true</enabled>
        <nodes>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
        </nodes>
      </param>
      <param name="CreditCardTariffs" description="Тарифы по кредитной карте">
        <type>service</type>
           <enabled>true</enabled>
        <nodes>
          <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="mobile.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node7.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="194.186.207.23">
            <enabled>true</enabled>
          </node>
        </nodes>
      </param>
      <param name="CreditCardDebtMid2019" description="Новый интерфейс задолженности по кредитной карте">
        <type>service</type>
           <enabled>true</enabled>
        <nodes>
          <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield2.online.sberbank.ru">
            <enabled>true</enabled>
           </node>
          <node id="mobile.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="194.186.207.23">
            <enabled>true</enabled>
          </node>
        </nodes>
      </param>
      <param name="AutorepaymentMid2019" description="Новый дизайн Автопогашения">
        <type>service</type>
           <enabled>true</enabled>
        <nodes>
          <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield2.online.sberbank.ru">
            <enabled>true</enabled>
           </node>
          <node id="mobile.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="ift-node7-mp.testonline.sberbank.ru">
            <enabled>false</enabled>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="194.186.207.23">
            <enabled>true</enabled>
          </node>
        </nodes>
      </param>
          <param name="MomentumCardEndDateMessage" description="Окончание срока действия карты Моментум">  
                <type>service</type>
                  <enabled>true</enabled>
           <nodes>
              <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="node4.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="greenfield2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="ift-node0-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
        </nodes>
       </param>
    
    <param name="MomentumCardEndDateMessageV2" description="Окончание срока действия карты Моментум НОВЫЙ, начиная с 9.6"> 
         <type>service</type>
         <enabled>true</enabled>
    </param>
      
    <param name="CurrencyCardBankDetail" description="Валютные реквизиты карты">
         <type>service</type>
         <enabled>true</enabled>
         <usdbanksdetail swift="IRVTUS3N" receivername="The Bank of New York Mellon, New York"/>
         <eurobanksdetail swift="DEUTDEFF" receivername="DEUTSCHE BANK AG, Frankfurt am Main"/>
    </param>
    
    <param name="MAppUpgradeCardDetails" description="Upgrade детальной информации по карте">
         <type>service</type>
         <enabled>true</enabled>
      
        <nodes>
        <node id="node0.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="node1.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="node2.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="node3.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="node4.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="greenfield1.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="greenfield2.online.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="mobile.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="ift-node1.testonline.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="ift-node2.testonline.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="ift-node1-mp.testonline.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="ift-node2-mp.testonline.sberbank.ru">
          <enabled>true</enabled>
        </node>

        <node id="194.186.207.23">
            <enabled>true</enabled>
        </node>
      </nodes>
    </param>
    
    <param name="MAppCardOwnerFullName" description="Отображение полной фамилии">
         <type>service</type>
         <enabled>true</enabled>   
    </param>

    <param name="EribStatePaymentShortCuts" description="Каталог бюджетных платежей - быстрый доступ к популярным услугам">
            <type>list</type>
            <shortcuts>
                <shortcut>
                    <title>Штрафы ГИБДД</title>
                    <icon>https://stat.online.sberbank.ru/PhizIC-res/logos/PU/7707089101.jpg</icon>
                    <nodes>
                        <node id="ift-node1-mp.testonline.sberbank.ru">
                            <catalogID>624234</catalogID>
                        </node>
                        <node id="ift-node0-mp.testonline.sberbank.ru">
                            <catalogID>624234</catalogID>
                        </node>
                        <node id="ift-node2-mp.testonline.sberbank.ru">
                            <catalogID>623567</catalogID>
                        </node>
                        <node id="ift-node1.testonline.sberbank.ru">
                            <catalogID>624234</catalogID>
                        </node>
                        <node id="ift-node2.testonline.sberbank.ru">
                            <catalogID>623567</catalogID>
                        </node>
                      	<node id="ift-node5.testonline.sberbank.ru">
                            <catalogID>623250</catalogID>
                        </node>
                      	<node id="ift-node5-mp.testonline.sberbank.ru">
                            <catalogID>623250</catalogID>
                        </node>
                      	<node id="psinode1.testonline.sberbank.ru">
                            <catalogID>688079</catalogID>
                        </node>
                      	<node id="mobile.sberbank.ru">
                            <catalogID>688079</catalogID>
                        </node>
                    </nodes>
                </shortcut>
                <shortcut>
                    <title>Налоги</title>
                    <icon>https://stat.online.sberbank.ru/PhizIC-res/IMG/PU/20/63/61/2b26d928c6b985710071f62251_38347.jpg</icon>
                    <nodes>
                        <node id="ift-node1-mp.testonline.sberbank.ru">
                            <catalogID>623139</catalogID>
                        </node>
                        <node id="ift-node0-mp.testonline.sberbank.ru">
                            <catalogID>617638</catalogID>
                        </node>
                        <node id="ift-node2-mp.testonline.sberbank.ru">
                            <catalogID>622021</catalogID>
                        </node>
                        <node id="ift-node1.testonline.sberbank.ru">
                            <catalogID>623139</catalogID>
                        </node>
                        <node id="ift-node2.testonline.sberbank.ru">
                            <catalogID>622021</catalogID>
                        </node>
                      	<node id="ift-node5.testonline.sberbank.ru">
                            <catalogID>622383</catalogID>
                        </node>
                      	<node id="ift-node5-mp.testonline.sberbank.ru">
                            <catalogID>622383</catalogID>
                        </node>
                    </nodes>
                </shortcut>
            </shortcuts>
        </param>
       <param name="NewBlockScreen" description="Новый экран заблокированной карты">
      <type>service</type>
           <enabled>true</enabled>       
       </param>
      <param name="MAppBlockCardReissueProcess" description="Досрочный перевыпуск заблокированных карт из детальной информации">
        <type>service</type>
           <enabled>true</enabled>       
       </param>
      	<param name="MobileBankSettings" description="Настройки для подключения МБ в МП">
    		<type>list</type>
            <MobileBankColdPeriodDuration>7 дней</MobileBankColdPeriodDuration>
    		<nodes>
				<node id="greenfield0.online.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                  
				</node>
              	<node id="greenfield1.online.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
                </node>
				<node id="psinode1.testonline.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="mobile.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="194.186.207.23">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="ift-node1.testonline.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="ift-node2.testonline.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="ift-node2-mp.testonline.sberbank.ru">
                  <mobileBankFromSetting>true</mobileBankFromSetting>
                  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
                  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
                  <mobileBankChangePhone>true</mobileBankChangePhone>
                  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
                  <ShowNotificationTerm>true</ShowNotificationTerm>
                  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
                  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>                                    
				</node>
				<node id="ift-node5-mp.testonline.sberbank.ru">
				  <mobileBankFromSetting>true</mobileBankFromSetting>
				  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
				  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
				  <mobileBankChangePhone>true</mobileBankChangePhone>
				  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
				  <ShowNotificationTerm>true</ShowNotificationTerm>
				  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
				  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>
				  <changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
				</node>
              	  <node id="ift-node7-mp.testonline.sberbank.ru">
				  <mobileBankFromSetting>true</mobileBankFromSetting>
				  <mobileBankFromCardSetting>true</mobileBankFromCardSetting>
				  <CardPhoneListCacheEnabled>true</CardPhoneListCacheEnabled>
				  <mobileBankChangePhone>true</mobileBankChangePhone>
				  <FullTariffTurnOffEnabled>true</FullTariffTurnOffEnabled>
				  <ShowNotificationTerm>true</ShowNotificationTerm>
				  <mobileBankActivateFlow_2>true</mobileBankActivateFlow_2>
				  <mobileBankDeactivateFlow_2>true</mobileBankDeactivateFlow_2>
				  <changePhoneAndTariffFromProfileEditor>true</changePhoneAndTariffFromProfileEditor>
				</node>
            </nodes>
        </param>
		<param name="overseastransferswift" description="Перевод на счет за рубеж через систему SWIFT">
            <type>list</type>
			<enabled>true</enabled>
			<commonErrorsProcessingEnabled>true</commonErrorsProcessingEnabled>
			<countryTransferBanEnabled description="Предупреждение о возврате">
				<enabled>true</enabled>
				<items>
					<item name="AU">Переводы в Австралию могут быть возвращены австралийскими банками. Продолжить?</item>
				</items>
			</countryTransferBanEnabled>
			<checkIbanSwiftEnabled description="Проверка значений IBAN SWIFT">
				<enabled>true</enabled>
				<items>
					<item name="DK">DK;FO;GL</item>
					<item name="FR">FR;MQ;GP;NC;RE;GF;PF;YT;PM;TF;WF;BL;MF</item>
					<item name="GB">GB;JE;IM</item>
					<item name="IE">IE;GB</item>
				</items>
			</checkIbanSwiftEnabled>
			<popularPurposesEnabled description="Раздел популярное">	
				<enabled>true</enabled>
				<items>
					<item name="id">14;12;14;15</item>
				</items>
			</popularPurposesEnabled>
		</param>
        <param name="a2aoverseastransferwutohide" description="Перевод денежных средств за границу через Western Union">
            <type>list</type>
            <enabled>true</enabled>
			<allRegions>0</allRegions>
			<countryVersionMappingEnabled>true</countryVersionMappingEnabled>
            <extendedFormEnabled>true</extendedFormEnabled>
			<countryVersionMappingEnabledNew>true</countryVersionMappingEnabledNew>
            <checkDetailsEnabled>true</checkDetailsEnabled>
            <AgreementLink>https://test.stat.online.sberbank.ru/WESTERNUNION/Oferta_Western_Union_a2a.pdf</AgreementLink>
			<WUViewTutorial description="Отображение туториала">
				<enabled>true</enabled>
				<countTutorial>1</countTutorial>
			</WUViewTutorial>
            <nodes>
                <node id="mobile.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
				<node id="ift-node0-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
				<node id="ift-node1-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
					<node id="ift-node7-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <INNWU>7727067410</INNWU>
                </node>
            </nodes>
        </param>
      	<param name="EribNewGibddCatalog" description="Новый каталог Госуслуги, Налоги, Штрафы, Пошлины на замену старого">
			<type>list</type>
			<nodes>
                <node id="ift-node1-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>1526</catalogID>
                </node>
                <node id="ift-node0-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>1526</catalogID>
                </node>
                <node id="ift-node2-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>2428</catalogID>
                </node>
                <node id="ift-node1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>1526</catalogID>
                </node>
                <node id="ift-node2.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>2428</catalogID>
                </node>
                <node id="ift-node5.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>2428</catalogID>
                </node>
              	<node id="ift-node5-mp.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>2428</catalogID>
                </node>
              	<node id="mobile.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>2351</catalogID>
                </node>
              	<node id="psinode1.testonline.sberbank.ru">
                    <enabled>true</enabled>
                    <catalogID>2351</catalogID>
                </node>
			</nodes>
		</param>
      <param name="PaymentsAndTransfers">
        <type>list</type>
        <paymentDetailPaymentMenuEnabled>true</paymentDetailPaymentMenuEnabled>
        <paymentCertificateBubbleEnabled>true</paymentCertificateBubbleEnabled>
        <paymentBillingProviderInvoiceInfo>true</paymentBillingProviderInvoiceInfo>
        <nodes>
          <node id="greenfield1.online.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>false</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>false</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="greenfield2.online.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
           </node>
           <node id="node1.online.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
           </node>
            <node id="node2.online.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
           </node>
           <node id="node3.online.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
           </node>
           <node id="node4.online.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
           </node>
          <node id="mobile.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="mobile2.sberbank.ru">
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
          </node>  
          <node id="ift-node1.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>false</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>false</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node7.testonline.sberbank.ru">
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>false</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>false</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node0-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>false</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>false</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentsVerifyUserPhoneNumber>true</paymentsVerifyUserPhoneNumber>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node3-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>false</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
           <node id="ift-node4-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>false</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node5-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentsVerifyUserPhoneNumber>true</paymentsVerifyUserPhoneNumber>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>
          <node id="ift-node7-mp.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentsVerifyUserPhoneNumber>true</paymentsVerifyUserPhoneNumber>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
            <paymentsAutoFillWithMask>true</paymentsAutoFillWithMask>
          </node>  
          <node id="psinode1.testonline.sberbank.ru">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <paymentsAutoFill>true</paymentsAutoFill>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
          	<paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
          </node>  
          <node id="194.186.207.23">
            <smartSearchFromPayment>true</smartSearchFromPayment>
            <BarcodeTutorialEnabled>true</BarcodeTutorialEnabled>
            <BarcodeScanIconEnabled>true</BarcodeScanIconEnabled>
            <QRCodeBubbleEnabled>true</QRCodeBubbleEnabled>
            <confirmationStatement>true</confirmationStatement>
            <paymentExternalCheckEnabled>true</paymentExternalCheckEnabled>
            <paymentExecTimeInfoEnabled>true</paymentExecTimeInfoEnabled>
            <paymentScanFileEnabled>true</paymentScanFileEnabled>
          </node>
        </nodes>
       </param>
<param name="ClientIncreaseLimitClaim" description="Увеличение индивидуального лимита для ВИП клиентов">
<type>service</type>
<increaseLimitEnabled>true</increaseLimitEnabled>
<nodes>
    <node id="node0.online.sberbank.ru">
    <enabled>true</enabled>
         <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="node1.online.sberbank.ru">
       <enabled>true</enabled>
         <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="node2.online.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="node3.online.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="greenfield1.online.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node1.testonline.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node2.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node7.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node1-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node0-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node2-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>  
    <node id="ift-node4-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="ift-node7-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="psinode2.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="psinode1.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitEnabled>true</increaseLimitEnabled>
    </node>
    <node id="mobile.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitEnabled>true</increaseLimitEnabled>
</node>
</nodes>
</param>
<param name="ClientIncreaseLimitBio" description="Увеличение индивидуального лимита для ВИП клиентов при помощи биометрии">
<type>service</type>
<increaseLimitBioEnabled>true</increaseLimitBioEnabled>
<nodes>
    <node id="node0.online.sberbank.ru">
    <enabled>true</enabled>
         <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="node1.online.sberbank.ru">
       <enabled>true</enabled>
         <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="node2.online.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="node3.online.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="greenfield1.online.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="ift-node1.testonline.sberbank.ru">
        <enabled>true</enabled>
          <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="ift-node2.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="ift-node1-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="ift-node0-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="ift-node2-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node> 
    <node id="ift-node4-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="ift-node7-mp.testonline.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="psinode2.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="psinode1.testonline.sberbank.ru">
        <enabled>true</enabled>
         <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
    </node>
    <node id="mobile.sberbank.ru">
        <enabled>true</enabled>
        <increaseLimitBioEnabled>true</increaseLimitBioEnabled>
	</node>
</nodes>
</param>
	  <param name="MessengerBeruGiftcard" description="Сертификаты Беру в диалогах">
		  <type>list</type>
		  <sendVersions>
			  <version name="9.11.0">
				  <enabled>true</enabled>
			  </version>
		  </sendVersions>
		  <receiveVersions>
			  <version name="9.11.0">
				  <enabled>true</enabled>
			  </version>
		  </receiveVersions>
          <agreements>
          	  <textSender>Приобретая подарочный сертификат, покупатель дает согласие ПАО Сбербанк на передачу своих персональных данных - ФИО и адреса электронной почты - маркетплейсу Беру (ООО "Яндекс Маркет")для оформления покупки подарочного сертификата.</textSender>
      	  </agreements>
          <nodes>
			  <node id="node0.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>684391</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="node1.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>684391</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="node2.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>500501445</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="node3.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>500500795</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="node4.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>500495145</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="greenfield1.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>550533493</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>http://j926608m.bget.ru/sites/default/files/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="greenfield2.online.sberbank.ru">
				  <billingID>284</billingID>
				  <providerID>550533493</providerID>
				  <serviceID>486042900175</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>http://j926608m.bget.ru/sites/default/files/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="194.186.207.23">
				  <billingID>284</billingID>
				  <providerID>635832</providerID>
				  <serviceID>635832</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="ift-node1.testonline.sberbank.ru">
				  <billingID>344</billingID>
				  <providerID>688848</providerID>
				  <serviceID>688848</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="ift-node1-mp.testonline.sberbank.ru">
				  <billingID>344</billingID>
				  <providerID>623383</providerID>
				  <serviceID>623383</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
              <node id="ift-node0-mp.testonline.sberbank.ru">
				  <billingID>344</billingID>
				  <providerID>623383</providerID>
				  <serviceID>623383</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="ift-node2-mp.testonline.sberbank.ru">
				  <billingID>344</billingID>
				  <providerID>623383</providerID>
				  <serviceID>623383</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="ift-node2.testonline.sberbank.ru">
				  <billingID>344</billingID>
				  <providerID>623383</providerID>
				  <serviceID>623383</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
			  <node id="mobile.sberbank.ru">
				  <billingID>344</billingID>
				  <providerID>688848</providerID>
				  <serviceID>688848</serviceID>
				  <accountEribFieldName>S356514975710A352998991921</accountEribFieldName>
                  <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
			  </node>
		  </nodes>
	</param>
    <param name="MessengerLitresGiftcard" description="Сертификаты ЛитРес в Диалогах">
    	<type>list</type>
    	<sendVersions>
          	  <version name="9.12.0">
				  <enabled>true</enabled>
			  </version>
		  </sendVersions>
		  <receiveVersions>
              <version name="9.8.0">
				  <enabled>true</enabled>
			  </version>
			  <version name="9.11.0">
				  <enabled>false</enabled>
			  </version>
              <version name="9.12.0">
				  <enabled>true</enabled>
			  </version>
    	</receiveVersions>
      	<agreements>
          	<textSender>Приобретая электронную книгу, покупатель дает согласие ПАО Сбербанк на передачу адреса электронной почты ООО "Препейд Солюшенс" для оформления покупки сертификата.</textSender>
          	<textReceiver>Я даю согласие ПАО Сбербанк на передачу номера мобильного телефона, используемого в мобильном приложении "Сбербанк Онлайн", ООО "ЛитРес" с целью авторизации или регистрации в личном кабинете онлайн-библиотеки ЛитРес.</textReceiver>
      	</agreements>
        <nodes>
            <node id="node0.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="node1.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="node2.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="node3.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="node4.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>http://j926608m.bget.ru/sites/default/files/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <billingID>284</billingID>
                <providerID>550538129</providerID>
                <serviceID>550538129</serviceID>
              	<accountEribFieldName>S503789069614A503789059641</accountEribFieldName>
            	<textEribFieldName>S503789069614A503789062082</textEribFieldName>
            	<dateEribFieldName>S503789069614A503789062597</dateEribFieldName>
                <catalogConfigUrl>http://j926608m.bget.ru/sites/default/files/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="194.186.207.23">
                <billingID>344</billingID>
                <providerID>688927</providerID>
                <serviceID>688927</serviceID>
              	<accountEribFieldName>S357407913386A357902514918</accountEribFieldName>
            	<textEribFieldName>S357407913386A357902514945</textEribFieldName>
            	<dateEribFieldName>S357407913386A357902514947</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="ift-node1.testonline.sberbank.ru">
                <billingID>344</billingID>
                <providerID>624158</providerID>
                <serviceID>624158</serviceID>
              	<accountEribFieldName>S202108599547A202900153557</accountEribFieldName>
            	<textEribFieldName>S202108599547A202900153562</textEribFieldName>
            	<dateEribFieldName>S202108599547A202900153560</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
                <billingID>344</billingID>
                <providerID>624158</providerID>
                <serviceID>624158</serviceID>
              	<accountEribFieldName>S202108599547A202900153557</accountEribFieldName>
            	<textEribFieldName>S202108599547A202900153562</textEribFieldName>
            	<dateEribFieldName>S202108599547A202900153560</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="ift-node0-mp.testonline.sberbank.ru">
                <billingID>344</billingID>
                <providerID>623567</providerID>
                <serviceID>623567</serviceID>
              	<accountEribFieldName>S202108599547A190216781206</accountEribFieldName>
            	<textEribFieldName>S202108599547A190216781214</textEribFieldName>
            	<dateEribFieldName>S202108599547A190216781217</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
                <billingID>344</billingID>
                <providerID>623567</providerID>
                <serviceID>623567</serviceID>
              	<accountEribFieldName>S202108599547A190216781206</accountEribFieldName>
            	<textEribFieldName>S202108599547A190216781214</textEribFieldName>
            	<dateEribFieldName>S202108599547A190216781217</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
                <billingID>344</billingID>
                <providerID>623567</providerID>
                <serviceID>623567</serviceID>
              	<accountEribFieldName>S202108599547A190216781206</accountEribFieldName>
            	<textEribFieldName>S202108599547A190216781214</textEribFieldName>
            	<dateEribFieldName>S202108599547A190216781217</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
            <node id="mobile.sberbank.ru">
                <billingID>344</billingID>
                <providerID>688927</providerID>
                <serviceID>688927</serviceID>
              	<accountEribFieldName>S357407913386A357902514918</accountEribFieldName>
            	<textEribFieldName>S357407913386A357902514945</textEribFieldName>
            	<dateEribFieldName>S357407913386A357902514947</dateEribFieldName>
                <catalogConfigUrl>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/iphonegiftsconfiguration.xml</catalogConfigUrl>
            </node>
        </nodes>
	</param>
    <param name="MessangerGiftsTab" description="Старый таб Подарок">
        <type>setting</type>
        <enabled>true</enabled>
	</param>
    <param name="MessengerGiftsTab" description="Старый таб Подарок в 9.8.0">
        <type>setting</type>
        <enabled>true</enabled>
	</param>
    <param name="GiftsBeruEnabled" description="Включение функционала отправки подарков от Беру.ру в Подарках">
    	<type>list</type>
        <smartSearchEnabled>true</smartSearchEnabled>
    	<sendVersions>
            <version name="9.12.0">
           		<enabled>true</enabled>
        	</version>
          	<version name="10.0.0">
           		<enabled>true</enabled>
        	</version>
            <version name="10.1.0">
           		<enabled>true</enabled>
        	</version>
    	</sendVersions>
    </param>
    <param name="GiftsLitresEnabled" description="Включение функционала отправки книг от ЛитРес в Подарках">
    	<type>list</type>
        <smartSearchEnabled>true</smartSearchEnabled>
    	<sendVersions>
            <version name="9.12.0">
           		<enabled>true</enabled>
        	</version>
          	<version name="10.0.0">
           		<enabled>true</enabled>
        	</version>
            <version name="10.1.0">
           		<enabled>true</enabled>
        	</version>
    	</sendVersions>
    </param>
  	<param name="MessengerGiftTab" description="Версионированный ключ для таба Подарок в Диалогах для версий с 9.13.0">
  		<type>list</type>
  		<enabled>true</enabled>
  		<sendVersions>
            <version name="9.12.0">
      			<enabled>true</enabled>
    		</version>
          <version name="10.0.0">
      			<enabled>true</enabled>
    		</version>
  		</sendVersions>
	</param>
  <param name="TelecomParameters" description="Телеком: Хост стенда, параметры доступа">
      <type>list</type>
      <nodes>
          <node id="node0.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="node1.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="node2.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="node3.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="node4.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="node5.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="greenfield1.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="greenfield2.online.sberbank.ru">
              <TelecomHost>https://api.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="194.186.207.23">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="ift-node0-mp.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="ift-node5-mp.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="mobile.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>false</TelecomWidgetAnalytics>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
              <TelecomHost>https://api-test.sberbank-tele.com/v2/</TelecomHost>
              <TelecomWidgetLimitsTabEnabled>true</TelecomWidgetLimitsTabEnabled>
              <TelecomWidgetAnalytics>true</TelecomWidgetAnalytics>
          </node>
      </nodes>
  </param>
	<param name="showTariffsLink" description="Пункт меню Тарифы, Лимиты и Сроки">
		<type>setting</type>
		<enabled>true</enabled>
		<link>
			https://stat.online.sberbank.ru/PhizIC-res/mapicfg/tariffs.xml
		</link>
  		<warningTextEnabled>true</warningTextEnabled>
		<warningText>Для операций в Сбербанке Онлайн. Полный перечень тарифов, лимитов и сроков осуществления переводов и платежей вы можете найти на сайте [www.sberbank.ru](https://www.sberbank.ru).</warningText>
	</param>
    <param name="interTransfer" description="Перевод в СНГ">
           <type>list</type>
           <enabled>false</enabled>
      	   <serviceProviders>
				<serviceProvider name="Western Union" visibleName="Western Union">
					<nodes>
                      <node id="ift-node1-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>623561</targetProvider>
							<targetService>623561</targetService>
						</node>
                        <node id="ift-node2-mp.testonline.sberbank.ru">
                            <targetBilling>344</targetBilling>
							<targetProvider>624932</targetProvider>
							<targetService>624932</targetService>
                        </node>
                        <node id="ift-node7-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>624320</targetProvider>
							<targetService>624320</targetService>
						</node>
                        <node id="mobile.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>5000641966</targetProvider>
							<targetService>5000641966</targetService>
						</node>
					</nodes>
				</serviceProvider>
           </serviceProviders>
           <checkName>Western Union</checkName>
           <minVersion>9.5</minVersion>
           <disabledForVersions>
              <disabledForVersion>9.5.0</disabledForVersion>
      	  </disabledForVersions>
      	   <!--Параметр showTutorial отвечает за доступность экрана Промо при входе в приложение-->
           <showTutorial>true</showTutorial>
      	   <!--Параметр WUTutorial отвечает за доступность и количество показов экрана Туториал при входе в операцию-->
           <WUTutorial description="Количество отображений Туториала">
              <enabled>true</enabled>
              <countTutorial>5</countTutorial>
           </WUTutorial>
           <links>
             <link name="additional">https://www.sberbank.ru/ru/person/remittance/perevod_po_nomery_telephona</link>
             <link name="offer">https://stat.online.sberbank.ru/WESTERNUNION/Offer_Transfers_for_CIS.pdf</link>
             <link name="otmena">https://test.stat.online.sberbank.ru/WESTERNUNION/otmena.pdf</link>
           </links>
           <deeplinkInterTransfer>false</deeplinkInterTransfer>
           <tarifPlans>
             <tarifPlan id="0"/>
		   </tarifPlans>
	</param>
    <param name="interTransferCancel" description="Отмена перевода для получения наличных в Western Union для версии 10.0">
           <type>list</type>
           <enabled>false</enabled>
      	   <serviceProviders>
				<serviceProvider name="Отмена Western Union" visibleName="Отмена Western Union">
					<nodes>
						<node id="ift-node1-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>123</targetProvider>
							<targetService>123</targetService>
						</node>
                        <node id="ift-node2-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>626744</targetProvider>
							<targetService>626744</targetService>
						</node>
                      	<node id="mobile.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>5000645498</targetProvider>
							<targetService>5000645498</targetService>
						</node>
                    </nodes>
                </serviceProvider>
           </serviceProviders>
    </param>
    <param name="interTransferCancelNew" description="Отмена перевода для получения наличных в Western Union для версии 10.1 и выше">
           <type>list</type>
           <enabled>true</enabled>
      	   <serviceProviders>
				<serviceProvider name="Отмена Western Union" visibleName="Отмена Western Union">
					<nodes>
						<node id="ift-node1-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>123</targetProvider>
							<targetService>123</targetService>
						</node>
                        <node id="ift-node2-mp.testonline.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>626744</targetProvider>
							<targetService>626744</targetService>
						</node>
                      	<node id="mobile.sberbank.ru">
							<targetBilling>344</targetBilling>
							<targetProvider>5000645498</targetProvider>
							<targetService>5000645498</targetService>
						</node>
                    </nodes>
                </serviceProvider>
           </serviceProviders>
    </param>
    <param name="AbroadTransferCashPayment" description="Перевод для получения наличных в Western Union">
        <type>setting</type>
        <enabled>true</enabled>
        <links>
			<link name="offer">https://stat.online.sberbank.ru/WESTERNUNION/Offer_Transfers_for_CIS.pdf</link>
		</links>
	</param>
    <param name="interTransferForeignBankToCard" description="Перевод в зарубежный банк на карту по НМТ">
           <type>list</type>
           <enabled>true</enabled>
           <nodes>
               <node id="ift-node1-mp.testonline.sberbank.ru">
                   <catalogID>1768</catalogID>
         </node>
               <node id="ift-node2-mp.testonline.sberbank.ru">
           <catalogID>2669</catalogID>
         </node>
               <node id="ift-node7-mp.testonline.sberbank.ru">
                   <catalogID>2650</catalogID>
         </node>
               <node id="ift-node0-mp.testonline.sberbank.ru">
                   <catalogID>2570</catalogID>
               </node>
             <node id="mobile.sberbank.ru">
                 <catalogID>5000002386</catalogID>
             </node>
           </nodes>
          <deeplinkForeignBankEnabled>true</deeplinkForeignBankEnabled>
          <historyNames>
              <historyName>Пeрeвoд в KБ "Kыpгызcтaн".</historyName>
              <historyName>Перевод в КБ "Кыргызстан".</historyName>
              <historyName>Пepeвoд в KБ "Kыpгызcтaн"</historyName>
              <historyName>Пepeвoд в Cпитaмeн Банк</historyName>
          </historyNames>
    </param>
    <param name="SelfEmployedV2" description="Сервис самозанятые">
    	<type>service</type>
   		<enabled>true</enabled>
    	<assignService>true</assignService>
   		<unassignService>true</unassignService>
    </param>  
    <param name="SelfEmployedV3" description="Сервис самозанятые">
    	<type>service</type>
   		<enabled>true</enabled>
    	<assignService>true</assignService>
   		<unassignService>true</unassignService>
    	<incomesListService>true</incomesListService>
      	<deleteIncomeService>true</deleteIncomeService>
		<addIncomeService>true</addIncomeService>
      	<autopayment>false</autopayment>
      	<addIncomeJur>true</addIncomeJur>
      	<links>
    		<link name="about">https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/selfemployed/tutorial.pdf</link>
    		<link name="offer">https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/selfemployed/semp_oferta.pdf</link>
  		</links>
    </param>  
    <param name="PersonalizationDDP" description="Персонализация от сервиса умного поиска">
    	<type>setting</type>
   		<enabled>true</enabled> 
    </param>
    <param name="authBlockingScreen" description="Выводить клиенту врем, через которое будет доступен вход в МП, после блокировки 5-значного пароля">
        <type>setting</type>
        <enabled>true</enabled>
    </param>
    <param name="singleCacheControlCenter" description="Механизм управления кэшом">
        <type>setting</type>
        <enabled>true</enabled>
    </param>
    <param name="NotificationsEnableSuggestion" description="">
		<type>setting</type>
		<enabled>true</enabled>
      	<periodInDays>1</periodInDays>
	</param>
    <param name="CreditCardInTransfersPermission" description="Управление запретом на использование кредитных карт в переводах p2p">
		<type>setting</type>
		<enabled>true</enabled>
		<nodes>
			<node id="node0.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node1.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node2.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node3.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node4.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="greenfield1.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="greenfield2.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
				<enabled>true</enabled>
			</node>
			<node id="mobile.sberbank.ru" description="Стенд ПСИ">
				<enabled>true</enabled>
			</node>
		</nodes>
	</param>
	<param name="ChangeVisibilityProduct" description="Частичное скрытие продукта">
			<type>setting</type>
			<enabled>true</enabled>
	</param>
	<param name="gsHideDeposits" description="Полное скрытие депозитов">
			<type>setting</type>
			<enabled>true</enabled>
	</param>
	<param name="gsHideIMs" description="Полное скрытие металлических счетов">
			<type>setting</type>
			<enabled>true</enabled>
	</param>
	<param name="gsHideProducts" description="Полное скрытие карт">
			<type>setting</type>
			<enabled>true</enabled>
	</param>
    <param name="RecoverProductVisibility" description="восстановление видимости продуктов в канале мобильное приложение">
			<type>setting</type>
			<enabled>true</enabled>
	</param>
    <param name="CyberSecurityEducation" description="Обучение в кабинете кибербезопасности">
    		<type>service</type>
    		<enabled>true</enabled>
	</param>
    <param name="ChangeAuthType" description="Настройка режима аутентификации при входе в интернет-банк">
    		<type>setting</type>   
    		<enabled>true</enabled>
	</param>
    <param name="TariffDebitCard" description="Тариф карты"> 
      <type>service</type>
         <enabled>true</enabled>
        <link>
             https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/card_tariffs.xml   
        </link>
      	<newLink>
        	 https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/card_tariffs_v2.xml 
        </newLink>
     <nodes>
        <node id="node0.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="node1.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="node2.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="node3.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="node4.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="greenfield1.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="greenfield2.online.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="mobile.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="ift-node1.testonline.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="ift-node2.testonline.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="ift-node1-mp.testonline.sberbank.ru">
          <enabled>false</enabled>
        </node>

        <node id="ift-node2-mp.testonline.sberbank.ru">
          <enabled>false</enabled>
        </node>
        <node id="psinode2.testonline.sberbank.ru">
          <enabled>false</enabled>
        </node>
        <node id="psinode1.testonline.sberbank.ru">
          <enabled>false</enabled>
        </node>
        <node id="194.186.207.23">
            <enabled>false</enabled>
        </node>
      </nodes>
    </param> 
    <param name="P2POverseasCardTransferExtended" description="Международный карточный перевод">
		<type>list</type>
		<enabled>true</enabled>
		<fixCurTransfer>true</fixCurTransfer>
		<viewExtendedInfo>true</viewExtendedInfo>
		<enabledLimitTransfer>true</enabledLimitTransfer>
		<limits>
			<error>Сумма одного перевода не должна превышать %1$s %2$s</error>
            <rur>150000</rur>
            <usd>2500</usd>
            <eur>2000</eur>
        </limits>
	</param>
      <param name="TargetBlockingCard" description="Целевая блокировка карты"> 
      	<type>service</type>
        <enabled>true</enabled>
       <nodes>
          <node id="node0.online.sberbank.ru">
            <enabled>false</enabled>
          </node>

          <node id="node1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="node2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="node3.online.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="node4.online.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="greenfield1.online.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="greenfield2.online.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="mobile.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="ift-node1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="ift-node2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="ift-node1-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="ift-node2-mp.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="psinode2.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>

          <node id="psinode1.testonline.sberbank.ru">
            <enabled>true</enabled>
          </node>
          <node id="194.186.207.23">
              <enabled>true</enabled>
        </node>
      </nodes>
    </param>
      <param name="MAppCardReissueProcess" description="Досрочный перевыпуск карты">
     		<type>service</type>
     		<enabled>true</enabled>
  			<nodes>
    			<node id="node0.online.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="node1.online.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="node2.online.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="node3.online.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="greenfield1.online.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="mobile.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="ift-node1.testonline.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="ift-node2.testonline.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="ift-node1-mp.testonline.sberbank.ru">
      				<enabled>true</enabled>
   				</node>

    			<node id="ift-node2-mp.testonline.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="psinode2.testonline.sberbank.ru">
      				<enabled>true</enabled>
    			</node>

    			<node id="psinode1.testonline.sberbank.ru">
      				<enabled>true</enabled>
    			</node>
    			<node id="194.186.207.23">
        			<enabled>true</enabled>
    			</node>
  			</nodes>
        </param>
      	
        <param name="VoiceAssistantPermissions" description="Голосовой помощник">
          <type>list</type>
          <enabled>true</enabled>
          <nodes>
            <node id="mobile.sberbank.ru">
              	<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
            
            <node id="greenfield1.online.sberbank.ru">
              	<NavigationBarEntryPointEnabled>false</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
            <node id="greenfield2.online.sberbank.ru">
              	<NavigationBarEntryPointEnabled>false</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
            
            <node id="psinode2.testonline.sberbank.ru">
      			<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet170.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
            	<SecondsPerChunk>1.0</SecondsPerChunk>
    		</node>
    		<node id="psinode1.testonline.sberbank.ru">
      			<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet170.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
            	<SecondsPerChunk>1.0</SecondsPerChunk>
    		</node>
            
            <node id="ift-node1.testonline.sberbank.ru">
              	<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
              	<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
              	<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
              	<NavigationBarEntryPointEnabled>true</NavigationBarEntryPointEnabled>
              	<SSLPinningEnabled>true</SSLPinningEnabled>
              	<VoiceProcessingServiceBaseURL>wss://renenet176.sigma.sbrf.ru:9443/vps/</VoiceProcessingServiceBaseURL>
              	<targetTapVoice>true</targetTapVoice>
              	<SecondsPerChunk>1.0</SecondsPerChunk>
            </node>
          </nodes>
        </param>
      
      <param name="ReceiverLayoutFromAddressBook" description="Функционал показа выбранного из адресной книги получателя включён">
		<type>setting</type>
		<enabled>true</enabled>
		<nodes>
			<node id="node0.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node1.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node2.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node3.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node4.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="greenfield1.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="greenfield2.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node1-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 1 (мобильный)">
				<enabled>true</enabled>
			</node>
			<node id="mobile.sberbank.ru" description="Стенд ПСИ">
				<enabled>true</enabled>
			</node>
		</nodes>
	</param>
     <param name="HotPhoneNumbers" description="Отображение горячих телефонов в МП">
 <type>setting</type>
 <hotPhonesEnabled>true</hotPhonesEnabled>
    <nodes>
      <node id="node0.online.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url></url>
      </node>
      <node id="node1.online.sberbank.ru">
	       <hotPhonesEnabled>true</hotPhonesEnabled>
        <url></url>
      </node>
      <node id="node2.online.sberbank.ru">
	       <hotPhonesEnabled>true</hotPhonesEnabled>
        <url></url>
      </node>
      <node id="node3.online.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url></url>
      </node>
      <node id="greenfield1.online.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url></url>
      </node>
      <node id="ift-node1.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="ift-node2.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="ift-node1-mp.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="ift-node0-mp.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="ift-node2-mp.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="ift-node4-mp.testonline.sberbank.ru">
	      <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="ift-node7-mp.testonline.sberbank.ru">
	      <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://ift-stat.testonline.sberbank.ru:4463/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="psinode2.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="psinode1.testonline.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/HotPhones_v1.xml</url>
      </node>
      <node id="mobile.sberbank.ru">
          <hotPhonesEnabled>true</hotPhonesEnabled>
        <url>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/HotPhones_v11.xml</url>
      </node>
      </nodes>
      </param>
      <param name="disabledFrameworks" description="Функционал отключения зависимостей">
   		 <enabled>true</enabled>
   		 <remoteToggleEnabled>true</remoteToggleEnabled>
			<disabledAnalytics>
				<analytics>Tune</analytics>        		
            </disabledAnalytics>
	</param>
		<param name="ChangeLocaleService" description="Многоязычность">
			<type>service</type>
			<languageSSMGChange>true</languageSSMGChange>
			<nodes>
    		<node id="node0.online.sberbank.ru">
       		<enabled>true</enabled>
         	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="node1.online.sberbank.ru">
       		<enabled>true</enabled>
         	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="node2.online.sberbank.ru">
        	<enabled>true</enabled>
          <languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="node3.online.sberbank.ru">
        	<enabled>true</enabled>
          <languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="greenfield1.online.sberbank.ru">
        	<enabled>true</enabled>
          <languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="ift-node1.testonline.sberbank.ru">
        	<enabled>true</enabled>
          <languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="ift-node2.testonline.sberbank.ru">
        	<enabled>true</enabled>
        	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="ift-node1-mp.testonline.sberbank.ru">
        	<enabled>true</enabled>
        	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="ift-node2-mp.testonline.sberbank.ru">
        	<enabled>true</enabled>
        	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="ift-node4-mp.testonline.sberbank.ru">
        	<enabled>true</enabled>
        	<languageSSMGChange>true</languageSSMGChange>
    		</node>
            <node id="ift-node7.testonline.sberbank.ru">
        	<enabled>false</enabled>
        	<languageSSMGChange>false</languageSSMGChange>
    		</node>
    		<node id="ift-node7-mp.testonline.sberbank.ru">
        	<enabled>false</enabled>
        	<languageSSMGChange>false</languageSSMGChange>
    		</node>
    		<node id="psinode2.testonline.sberbank.ru">
        	<enabled>true</enabled>
         	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="psinode1.testonline.sberbank.ru">
        	<enabled>true</enabled>
         	<languageSSMGChange>true</languageSSMGChange>
    		</node>
    		<node id="mobile.sberbank.ru">
      	  <enabled>true</enabled>
        	<languageSSMGChange>true</languageSSMGChange>
				</node>
			</nodes>
		</param>
		<param name="ManagerRegistration" description="регистрация менеджера в всп">
			<type>setting</type>
			<enabled>true</enabled>
		</param>
        <param name="hideOperationsCardCLIENT2OTHER"  description="Скрытие операций по дополнительной карте, которые должны быть недоступны для держателя основной карты">
          <type>setting</type>
          <enabled>true</enabled>
        </param>
        <param name="CloseCardAccount" description="Закрытие счета карты"> 
        	<type>service</type>
             <enabled>true</enabled>
             <nodes>               
                <node id="mobile.sberbank.ru">
                  <enabled>true</enabled>
                </node>

                <node id="ift-node1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>

                <node id="ift-node2.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>

                <node id="ift-node1-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>

                <node id="ift-node2-mp.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>

                <node id="psinode2.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>

                <node id="psinode1.testonline.sberbank.ru">
                  <enabled>true</enabled>
                </node>
                <node id="194.186.207.23">
                    <enabled>true</enabled>
                </node>
              </nodes>
    </param>
    <param name="iscServiceDetails"  description="Отображения условий обслуживания по картам ИЗК">
		<type>setting</type>
		<enabled>true</enabled>
		<link>https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/levels_isc.xml</link>
	</param>
    <param name="UseTransferFromCreditCard101"  description="Доступность выбора кредитной карты как источника списания в переводах между своими счетами">
        <type>setting</type>
        <enabled>true</enabled>
    </param>
<param name="mobileQuickPayment" description="Быстрые суммы при оплате сотового">
      <type>setting</type>
      <enabled>true</enabled>
      <quickpayments>
          <quickpayment>100</quickpayment>
          <quickpayment>200</quickpayment>
          <quickpayment>500</quickpayment>
      </quickpayments>
      <nodes>
          <node id="node0.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node1.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node2.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node3.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="node4.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="greenfield1.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="greenfield2.online.sberbank.ru">
              <enabled>true</enabled>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru" description="Стенд ИФТ блок 2 (мобильный)">
              <enabled>true</enabled>
          </node>
          <node id="mobile.sberbank.ru" description="Стенд ПСИ">
               <enabled>true</enabled>
          </node>
      </nodes>
    </param>      
	<param name="GeolocationFeatures" description="Данные по банкоматам на карте">
    <type>list</type>
         <showPhone>false</showPhone>
         <showAddress>false</showAddress>
         <showStatus>false</showStatus>
	</param>
    <param name="persAnimation" description="personal animation">
			<defaultAnimationEnabled>true</defaultAnimationEnabled>
			<persAnimationEnabled>true</persAnimationEnabled>
      		<classicViewEnabled>false</classicViewEnabled>
      		<randomAnimation>true</randomAnimation>
      		<animationUrls>
				<animationUrl url="https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/logonanimation/ios_animation_config.xml" fileVersion="4" version="9.13.0"/>
              	<animationUrl url="https://test.stat.online.sberbank.ru/PhizIC-res/mapicfg/logonanimation/ios_animation_config_randomizer.xml" fileVersion="1" version="10.2.0"/>
            </animationUrls>
	</param>
    <param description="Шапка на главной с Next Best Actions" name="DDAMainWidgetPermissions">
      <defaultActiveTab>1</defaultActiveTab>
      <list>
          <value>p2p</value>
		  <value>p2p_default</value>
		  <value>qr</value>
		  <value>loyalty</value>
		  <value>provider</value>
		  <value>total_finances</value>
		  <value>budget</value>
		  <value>alf</value>
		  <value>salary</value>
      </list>
      <nodes>
          <node id="node0.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="node1.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="node2.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="node3.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="node4.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="greenfield1.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
		          <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="greenfield2.online.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="mobile.sberbank.ru">
              <list>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="ift-node1.testonline.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="ift-node2.testonline.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="ift-node1-mp.testonline.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="ift-node2-mp.testonline.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="psinode2.testonline.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="psinode1.testonline.sberbank.ru">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
          <node id="194.186.207.23">
              <list>
                  <value>p2p</value>
		  		  <value>p2p_default</value>
				  <value>qr</value>
				  <value>loyalty</value>
				  <value>provider</value>
				  <value>total_finances</value>
				  <value>budget</value>
				  <value>alf</value>
				  <value>salary</value>
              </list>
          </node>
      </nodes>
    </param>
    <param name="NewBlockCardScreen" description="Новый экран заблокированной карты"> 
  <type>service</type>
     <enabled>true</enabled>
 <nodes>
    <node id="node0.online.sberbank.ru">
      <enabled>true</enabled>
    </node> 
    <node id="node1.online.sberbank.ru">
      <enabled>true</enabled>
    </node> 
    <node id="node2.online.sberbank.ru">
      <enabled>true</enabled>
    </node> 
    <node id="node3.online.sberbank.ru">
      <enabled>true</enabled>
    </node>     
    <node id="node4.online.sberbank.ru">
      <enabled>true</enabled>
    </node>     
    <node id="greenfield1.online.sberbank.ru">
      <enabled>true</enabled>
    </node>    
    <node id="greenfield2.online.sberbank.ru">
      <enabled>true</enabled>
    </node>
    <node id="mobile.sberbank.ru">
      <enabled>true</enabled>
    </node>
    <node id="ift-node1.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
     <node id="ift-node2.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
     <node id="ift-node1-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
    <node id="ift-node2-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
     <node id="psinode2.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
     <node id="psinode1.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
    <node id="194.186.207.23">
        <enabled>true</enabled>
    </node>
  </nodes>      
</param>
	<param name="TransferDesign2019" description="Новый дизайн меню переводов 2019">
    <enabled>true</enabled>
	<showTutorial>false</showTutorial>
    <nodes>
         <node id="greenfield1.online.sberbank.ru">
             <enabled>true</enabled>
         </node>
         <node id="mobile.sberbank.ru">
             <enabled>true</enabled>
         </node>
         <node id="ift-node1-mp.testonline.sberbank.ru">
             <enabled>true</enabled>
         </node>
         <node id="ift-node2-mp.testonline.sberbank.ru">
             <enabled>true</enabled>
         </node>
         <node id="ift-node7-mp.testonline.sberbank.ru">
             <enabled>true</enabled>
         </node>
    </nodes>
	</param>
    <param name="CardUnblocking" description="Разблокировка карты">  
  <type>service</type>
     <enabled>true</enabled>
 <nodes>
    <node id="node0.online.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="node1.online.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="node2.online.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="node3.online.sberbank.ru">
      <enabled>true</enabled>
    </node>
    
	<node id="node4.online.sberbank.ru">
      <enabled>true</enabled>
    </node>
    
	<node id="greenfield1.online.sberbank.ru">
      <enabled>true</enabled>
    </node>
	
	<node id="greenfield2.online.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="mobile.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="ift-node1.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="ift-node2.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
   
    <node id="ift-node1-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="ift-node2-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
   
 	<node id="ift-node5-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
   
    <node id="psinode2.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>

    <node id="psinode1.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
	<node id="194.186.207.23">
    	<enabled>true</enabled>
	</node>
  </nodes>
</param>
     <param name="MultiCurrencyCard" description="Мультивалютная карта в МП"> 
  <type>service</type>
     <enabled>true</enabled>
 <nodes>    
    <node id="mobile.sberbank.ru">
      <enabled>true</enabled>
    </node>
 
    <node id="ift-node1.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
 
    <node id="ift-node2.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
 
    <node id="ift-node1-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
 
    <node id="ift-node2-mp.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
 
    <node id="psinode2.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
 
    <node id="psinode1.testonline.sberbank.ru">
      <enabled>true</enabled>
    </node>
    <node id="194.186.207.23">
        <enabled>true</enabled>
    </node>
  </nodes>	
	</param>
        <param name="Autopayment" description="Функционал Автоплатежей">
		    <enabled>false</enabled>
		    <autoAllOperations>false</autoAllOperations>
		    <moneyBoxes>false</moneyBoxes>
		    <nodes>
		        <node id="node0.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="node1.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="node2.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="node3.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="node4.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="greenfield1.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="greenfield2.online.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="194.186.207.23">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="mobile.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="psinode0.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="psinode1.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="psinode2.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node0.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node1.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node2.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node0-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node1-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node2-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node3-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node4-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node5-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="ift-node7-mp.testonline.sberbank.ru">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		        <node id="10.21.152.7">
		            <enabled>true</enabled>
                    <autoAllOperations>true</autoAllOperations>
              	    <moneyBoxes>false</moneyBoxes>
		        </node>
		    </nodes>
        </param>
    <param name="EscrowAccounts" description="Эскроу счета">
        <type>list</type>
        <enabled>false</enabled>
        <nodes>
            <node id="node0.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node3.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="node4.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield1.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="greenfield2.online.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="mobile.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node3.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node1-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node2-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node4-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node5-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="ift-node7-mp.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode2.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="psinode1.testonline.sberbank.ru">
                <enabled>true</enabled>
            </node>
            <node id="194.186.207.23">
                <enabled>true</enabled>
            </node>
        </nodes>
    </param>
    <param name="SbercardServiceDetails" description="Доступность функционала Сберкарты 2.0">
      <type>list</type>
      <enabled>true</enabled>
      <disabledForVersions>
        <version>9.5.0</version>
      </disabledForVersions>
    </param>
	<param name="preloginAlert" description="Предупреждение клиента перед входом о возможных проблемах">
    	<enabled>true</enabled>
    	<link>https://test.stat.online.sberbank.ru/SALESTOOLS/offers/alerts-android.xml</link>
	</param>
    <param name="AccessibilityMarkersClaim" description="Анкета о специальном обслуживании">
		<type>setting</type>
		<enabled>true</enabled>
		<nodes>
			<node id="node0.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node1.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node2.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node3.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="node4.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="greenfield1.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="greenfield2.online.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="mobile.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node1.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node2.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node3.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node4.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node1-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node2-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node4-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node5-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="ift-node7-mp.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="psinode2.testonline.sberbank.ru">
				<enabled>true</enabled>
			</node>
			<node id="psinode1.testonline.sberbank.ru"> 
				<enabled>true</enabled>
			</node>
		</nodes>
	</param>
    <param name="VoiceOverHeader" description="Право на включение voice over в расширенном заголовке на главном">
		<enabled>true</enabled>
	</param>
    <param name="DifferentiatedTariffsCommission" description="Отображение новой комиссии для дифтарифов">
		<enabled>true</enabled>
	</param>
  </params>
</configuration>
