<!DOCTYPE html>
<html>
   <head>
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <style>
         * {
         box-sizing: border-box;
         }
         body {
         background-color: #474e5d;
         font-family: Helvetica, sans-serif;
         }
         /* The actual timeline (the vertical ruler) */
         .timeline {
         position: relative;
         max-width: 1200px;
         margin: 0 auto;
         }
         /* The actual timeline (the vertical ruler) */
         .timeline::after {
         content: '';
         position: absolute;
         width: 6px;
         background-color: white;
         top: 0;
         bottom: 0;
         left: 50%;
         margin-left: -3px;
         }
         /* Container around content */
         .container {
         padding: 10px 40px;
         position: relative;
         background-color: inherit;
         width: 50%;
         }
         /* The circles on the timeline */
         .container::after {
         content: '';
         position: absolute;
         width: 25px;
         height: 25px;
         right: -17px;
         background-color: white;
         border: 4px solid #FF9F55;
         top: 15px;
         border-radius: 50%;
         z-index: 1;

         }
         /* Place the container to the left */
         .left {
         left: 0;
         }
         /* Place the container to the right */
         .right {
         left: 50%;
         }
         /* Add arrows to the left container (pointing right) */
         .left::before {
         content: " ";
         height: 0;
         position: absolute;
         top: 22px;
         width: 0;
         z-index: 1;
         right: 30px;
         border: medium solid white;
         border-width: 10px 0 10px 10px;
         border-color: transparent transparent transparent white;
         }
         /* Add arrows to the right container (pointing left) */
         .right::before {
         content: " ";
         height: 0;
         position: absolute;
         top: 22px;
         width: 0;
         z-index: 1;
         left: 30px;
         border: medium solid white;
         border-width: 10px 10px 10px 0;
         border-color: transparent white transparent transparent;
         }
         /* Fix the circle for containers on the right side */
         .right::after {
         left: -16px;
         }
         /* The actual content */
         .content {
         padding: 20px 30px;
         background-color: white;
         position: relative;
         border-radius: 6px;
         }
         /* Media queries - Responsive timeline on screens less than 600px wide */
         @media screen and (max-width: 600px) {
         /* Place the timelime to the left */
         .timeline::after {
         left: 31px;
         }
         /* Full-width containers */
         .container {
         width: 100%;
         padding-left: 70px;
         padding-right: 25px;
         }
         /* Make sure that all arrows are pointing leftwards */
         .container::before {
         left: 60px;
         border: medium solid white;
         border-width: 10px 10px 10px 0;
         border-color: transparent white transparent transparent;
         }
         /* Make sure all circles are at the same spot */
         .left::after, .right::after {
         left: 15px;
         }
         /* Make all right containers behave like the left ones */
         .right {
         left: 0%;
         }
         .collapsible {
         background-color: #777;
         color: white;
         cursor: pointer;
         padding: 18px;
         width: 100%;
         border: none;
         text-align: left;
         outline: none;
         font-size: 15px;
         }
         .active, .collapsible:hover {
         background-color: #555;
         }
         .span.a {
         padding: 0 18px;
         display: none;
         overflow: hidden;
         background-color: #f1f1f1;
         }
         }
      </style>
      <script>
         var coll = document.getElementsByClassName("collapsible");
         var i;
         
         for (i = 0; i < coll.length; i++) {
           coll[i].addEventListener("click", function() {
             this.classList.toggle("active");
             var content = this.nextElementSibling;
             if (content.style.display === "block") {
               content.style.display = "none";
             } else {
               content.style.display = "block";
             }
           });
         }
      </script>
   </head>
   <body>

<div>
<p>The details were mainly taken from the book, "When the Moon Split" compiled by Safiur Rahman Mubarakpuri. Other additional information were taken from other sources such as <a href="https://www.islamicbulletin.org">Link</a></p>
</div>

      <div class="timeline">
         
		  
		 
		 
		 
		 
		 <div class="container right">
            <div class="content">
               <h2>Prophet Ibrahim / Abraham (As)</h2>
               <p>
               <ul>
                  


				  <li><a href="https://quran.com/21/58">Breaks Idols</a></li>
                  <li>Father thorws him out of the home</li>
                  <li>Goes for in search of God</li>
                  <li>King throws Ibrahim (As) in fire</li>
                  
				  <li><a href="https://quran.com/3/173">Ibrahim (As) says "HabunAllah owa ni maal owakeel", more or less meaning, "Allah alone is sufficient as an aid for us and He is the best Protector." And Allah knows the best</a></li>
				  
                  <li>His relative Prophet Lut (As) also gets prophethood</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>Good news of Son</h2>
               <p>
               <ul>
                  
				  <li><a href="https://quran.com/11/71">Angel visits and gives good news of son to Ibrahim (As)</a></li>
				  
                  <li>Yaqoob and Ishmael (As) are the two sons</li>
                  <li>From Prophet Yaqoob (As) comes Bani Israel and all their Prophets, including Prophet Isa / Jesus, Prophet Musa / Moses peace be upon all off them</li>
                  <li>Prophet Muhammad (pbuh) comes fromt he lineage of Prophet Ishmael (As)</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>Ibrahim (As) goes to Makkah</h2>
               <p>
               <ul>
                  <li>Leaves Sarah and Ishmael (As)</li>
                  <li>Angel comes and by the will of Allah forms the ZamZam well near baby Ishmael (As)</li>
                  <li>A tribe from Yemen (Jurhum) comes and settles there</li>
                  <li>Life begins at Makkah</li>
                  <li>Ibrahim and Ishmael (As) builds Kabah</li>
               </ul>
               </p>
            </div>
         </div>
		 
		 <div class="container left">
            <div class="content">
               <h2>Jews in Medina</h2>
               <p>
               <ul>
                  <li>There were Jews in Madina before Prophet pbuh</li>
                  <li>They were waiting for their prophet and were looking for a place the description of which matched Madina</li>
                  <li>Allah mentions in the Quran about them, they knew the Prophet pbuh more than their own children</li>

               </ul>
               </p>
            </div>
         </div>
		 
		 
         <div class="container left">
            <div class="content">
               <h2>Qusai Ibn Qalb</h2>
               <p>
               <ul>
                  <li>His lineage was from Prophet Ishmael (As)</li>
				  <li>He went to top of the chain by uniting the Qurayesh tribe</li>
				  <li>He gained power over Khujaya tribe</li>
                  <li>His sons are going to be the leaders of Qurayesh</li>
                  <li>They (i.e. his sons) will have duties and responsibilities of taking care of Hajjis</li>
				  <li>One of his son was Abde Manaf</li>
				  <li>Abde Manaf had a son named, Haashim</li>
				  <li>Haashim's son Abdul Muttalib is the Grand Father of Prophet pbuh</li>
				  <li>In other words, Son of Abdul Muttalib is Abdullah, and Son of Abdullah is Prophet pbuh</li>
				  <li>People of Qurayesh were honoured because they were the caretakers of the Kabah</li>
				  
               </ul>
               </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>Abdul Muttalib</h2>
               <p>
               <ul>
                  <li>Abraha attacks Kaba</li>
                  <li>Abdul Muttalib prays to Allah to save Kaba</li>
                  <li>Allah sends small birds to attack the army of Abraha</li>
                  <li>This year is recorded in verbal history as the year of fill (Elephants)</li>
                  <li>Zurhum hides ZamZam before fleeing</li>
                  <li>Abdul Muttalib sees a dream and gets inspired to dig and find ZamZam again</li>
                  <li>Abdul Muttalib prays for more sons</li>
                  <li>Abdul Muttalib was blessed with more sons and as per his promise he goes to sacrifice Abdullah, the father of Prophet (pbuh)</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>His (pbuh) father</h2>
               <div>
                  <p>Prophet (pbuh)'s father died few months before he (pbuh) was born. Approximately on 570 CE. (Require Verification)</p>
               </div>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>571 Year of Birth</h2>
               <p>571 CE, Prophet pbuh was born as per "When the Moon Split" compilled by S R Mubarakpuri</p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>Brought up by Grandfather and Mother</h2>
               <p>Ameena and Abdul Muttalib</p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>Haleema Sa'dya (Ra)</h2>
               <p>
               <ul>
                  <li>Makkan's had a tradition of sending young kids to deserts for learning pure language and to be tough in the harsh environment</li>
                  <li>Haleema (Ra) was one of the foster mothers who was looking for a baby to take care</li>
				  <li>Haleema (Ra) finds blessings in her body, animals and they could spot the goodness as soon as the Prophet pbuh went to their house</li>
                  <li>None took Prophet pbuh as he pbuh was an orphan, except Haleema(Ra)</li>
                  <li>During his pbuh stay at Haleema (Ra) (Ra) the incident with Angel Gibrael took place where he came and washed his (pbuh) heart as per the hadith. Narrated by Muslim (162)</li>
				  
               </ul>
               </p>



            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>Losing Mother and Grandfather</h2>
               <ul>
                  <li>After coming back from Haleema (Ra), Prophet pbuh stayed with his pbuh mother approximately 2 years</li>
				  <li>After that his pbuh mother died</li>
				  <li>Then for sometime Prophet pbuh was under the care of his pbuh, Grandfather</li>
				  <li>After the Grandfather passed away the Prophet pbuh was looked after by his pbuh Uncle Abu Talib, the son of Abdul Muttalib</li>
                  
				  
               </ul>
            </div>
         </div>
         
         <div class="container left">
            <div class="content">
               <h2>Before Marriage</h2>
               <p>as per "When the Moon Split" compilled by S R Mubarakpuri:
               <ul>
                  <li>At the age of 12 Prophet (pbuh) went to Syria with his (pbuh) uncle Abu Talib</li>
                  <li>A christian monk named as Bahira recognised Prophet (pbuh) as having sings of being a prophet</li>
                  <li>Bahira warned Abu talib to take the Prophet (pbuh) at a safe place in case the Bizentines finds out about him and kill him</li>
                  <li>Prophet pbuh participated Battle of Fijar at the age of 20 on the side of Qurayesh</li>
                  <li>Hilf ul Fudul was formed</li>
                  <li>Like all other prophets, our Prophet pbuh also tended sheep for sometime for the people of Makkah</li>
				  <li>Khadeejaa (Ra) appoints Prophet pbuh as her business representative to Syria</li>
		
				  
               </ul>
               </p>
            </div>
         </div>
         
         <div class="container left">
            <div class="content">
               <h2>596 Marriage with Khadeeja (Ra)</h2>
               
               <ul>
                  <li>Khadeeja (Ra) gets very impressed by the character and truthfulness of the Prophet pbuh</li>
				  <li>Khadeeja offers to marry Prophet pbuh</li>
				  
				  
				  <ul>
				  Over the nex few years, Prophet pbuh gets blessed with four daughters:
				  <li>Birth of first daugher Zainaab (Ra)</li>
                  <li>Birth of second daugher Ruqaiya (Ra)</li>
                  <li>Birth of third daugher Umm Kulthum (Ra)</li>
                  <li>Birth of fourth daugher Fatimah (Ra)</li>
				  </ul>
				  
				  
				  
				  
				  
				  
               </ul>
               
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>Placement of Blackstone and resolving the conflicts</h2>
               <p> 
			   
			                  <ul>
                  <li>Qurayesh tribs were about to fight eachother on the issue of who will place the holy blackstone at its place after the reconstruction of Kabah</li>
                  <li>Prophet pbuh solved this issue by using a big cloth and advising the fighting tribes to hold each corners</li>
                  <li>He pbuh placed the stone by himself pbuh</li>
                  <li>Everyone was happy to see Al Ameen to resolve the issue, they loved the Prophet for his noble character and truthfulness (pbuh)</li>
               </ul>
			   
			   
			   </p>
            </div>
         </div>
        
         <div class="container right">
            <div class="content">
               <h2>610 CE, First Revelation</h2>
               <p>First Revelation, during the month of Ramadan (Verification Required)
			   <ul>
			   <li>Throughout his pbuh life, Allah kept him pbuh away from shirk and paganism</li>
			   <li>Prophet pbuh used to to away from all the corruption of the Makkan society and seek refuge in solitude in the cave of Hira</li>
			   <li>During one of these sessions was the first time Allah sent Gibrael (As) with the verses of Surah Alak, the first revealation at the age of 40</li>
			   <li><a href="https://quran.com/96/1">It was not an accident or coincidence the the first verse revelaed was an advise to read, i.e. "Iqra"</a></li>
			   
			   <li>Reading / gaining knowldege is the foundation of seeking guidance and worship Allah with the correct knowledge</li>
			   <li>Prophet pbuh was scared and shocked to experience the appearance of Gibarel (As)</li>
				<li>Prophet pbuh told this to his pbuh wife Khadeeja (Ra)</li>
				<li>Khadeeja (Ra)immediately beleived Prophet pbuh, and became the first ever Muslim on the face of Earth, what an honor</li>
			   <li>Secret Preaching started</li>
			   
				
			   </ul>
			   
			   
			   
			   </p>
            </div>
         </div>
		 
		 <div class="container right">
            <div class="content">
               <h2>First few beleivers</h2>
               
			   <ul>
			   
			   <li>After Khadeeja (Ra), Ali (Ra) and his pbuh daughers were among the first beleivers</li>
			   <li>Abu Bakar (Ra) was the first Muslim outsite of Prophet (pbuh) family</li>
			   <li>Abu Bakar was his pbuh neighbour and friend</li>
			   <li>Makkans used to love Abu Bakar (Ra) for his noble character which was similar to Prophet pbuh, no wonder they were friends and were almost of same age (i.e. one year difference approximately)</li>
		
				
			   </ul>
			   
			   
			   
			   
            </div>
         </div>
		 
		 
		 
		   <div class="container left">
            <div class="content">
               <h2>Makkans Reaction</h2>
               
			   <ul>
			   <li>Makkans didnt accept the message of Prophet pbuh</li>
			   <li>Makkans were not going to give up the religion, custom and culture of their forefathers</li>
			   <li>Makkans started punishing their Muslim slaves</li>
			   <li>These tourture only raised the status of the Companions (Ra) of the Prophet pbuh</li>
			   <li>Leaders of Qurayes tribe tries to talk to Abu Talib, the Uncle of the Prophet pbuh for Prophet to refrain from preaching</li>
			<li>Abu Talib did not back off and showed unconditional support to his nephew pbuh</li>
			   <li>614 Sumayia's death</li>
			   <li>615 First migration to Abisynia</li>
			   <li>615 Hamza (Ra) joins in the group of First Muslims</li>
			   <li>616 Omar (Ra) joins in the group of First Muslims</li>
			   <li>Religion of Islam became strong after these two men joined in and beleived in the message</li>
			   <li>Muslims prayed openly at the Kabah</li>
<li>They openly declared their faith</li>
			   
				
			   </ul>
			   
			   
			   
			   
            </div>
         </div>
		 
         

		   <div class="container left">
            <div class="content">
               <h2>Dawah strategy at Makkah</h2>
               
			   <ul>
<p>In his book "When the Moon Split" Safiur Rahman Mubarakpuri points out some of the hikmah of the way the Prophet pbuh and companions dealt with the opression, however Allah knows the best</p>

			   <li>The companions (Ra) were being trained to face the torture and punishment on the path of Allah</li>
			   <li>They were able to endure due to their lack of attachment with the Duniya and eagerness for the bliss of Paradise</li>
			   <li>They were positive about the future of Islam knowing and beleiving that Allah will complete the matter and make Islam the dominant religion of God on the face of Earth</li>
			   <li>Peaceful preaching was effective in Makkah instead of fighting as that would trigger hatered and more bloodshed instead of the spread of the message</li>
			   <li>Fighting between Qurayesh and Muslims would mean to the outsiders that Islam came to initiate fight amongst family members</li>
			   <li>Muslims were few in numbers so the message would get hard to get outside of Arabia if all were engaged in fighting and getting killed at that stage</li>
			   <li>There was no real need for fighting as Islam was growing slowly but steadily</li>



			   
				
			   </ul>
			   
			   
			   
			   
            </div>
         </div>

         <div class="container left">
            <div class="content">
               <h2>Few points on migration to Abisineya</h2>
               <p>
               <ul>
                  <li>Prophet pbuh wanted to save and ensure the spread of the message and hence he sent some Mulsims to a land of just king</li>
                  <li>People of Abissinya were Christians (Abrahamic Religion) opposed to the people of Makkah who were pagans this was an advantage for Muslims</li>
                  <li>Prophet pbuh knew about Abissinya from his pbuh nursemaid Umm Aiman about the land and its people</li>
                  <li>As a merciful Leader Prophet pbuh was concerned about the safety and freedom of his pbuh followers and hence he pbuh permitted Hijrah option for them to go and live a safe life and spread the message</li>
<li>In the group there were Companions (Ra) like his pbuh dauther (Rukaiya Ra), son in law (Uthman Ra) and his pbuh cousin Jafar ibn Abu Taleb, which shows he pbuh was not taking a mere chance wih the life of some followers and including his pbuh beloved family members in that decision too</li>
<li>This also shows even though his pbuh family members had to suffer the same fate as his followers / companions (Ra)</li>
<li>These migrations (1st and 2nd Abissinyan migrations) lowered the status of Qurayesh as others in Surrounding areas were kind eough to provide shelter to their (Qurayesh's own tribesmen) people. And it als became obvious they (Qurayesh) were prosecuting Muslims because they worship only Allah and no one else</li>
<li>...</li>

               </ul>
               </p>
            </div>
         </div>
			   
			   
         
         <div class="container left">
            <div class="content">
               <h2>618 Boycott of Banu Hasheem by Qurayesh</h2>
               <p>
			   
			   
			   
			    <ul>
			   <li>3 years boycott</li>
			   <li>Including Abu Talib and Khadeeja and their children go through severe pain for not having adequate food and supplies</li>
			   <li>Amazing stories of companions are heard on how they used to live on very little during this time</li>
			   <li>How Prophet (pbuh) might have been feeling for putting his (phuh) in this and not being able to do anything for them subhanAllah!</li>
			   <li>Insects ate everyting on the treaty that stated the boycott excepth the word in the name of Allah (God) which was kep inside Kabah (ref required)</li>
			   
			   	
				
			   </ul>
			   
			   
			   
			   
			   </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>619 Losing Wife and Uncle</h2>
			   
			   <p>
			   <ul>
			   <li>Age 49</li>
			   <li>A group goes for second Migration to Abisynia</li>
			   <li>Death of Abu Talib, the Uncle</li>
			   <li>Death of Khadeeja (Ra)</li>
			   <li>Taif Visit</li>
			   </ul>
			   	   
               </p>
            </div>
         </div>
         
         
         <div class="container right">
            <div class="content">
               <h2>620 Isra al Miraaj</h2>
               <p>
			   
			    
			   
			   <ul>
			   <li>Age 50</li>
			   <li><a href="https://quran.com/17/1">Firstly Prophet pbuh goes from Makkah to Jerujalem and from there to Heaven</a></li>
			   <li>Prayer was revealed</li>
			   <li>Last few verses of Surah Bakarah was revealed (verification required)</li>
			   <li></li>
			   <li>Abu Bakar (Ra) says, if he (pbuh) says he (pbuh) went to Jerusalem, then he (pbuh) is saying the truth</li>
			   <li>Prophet (pbuh) narrates baitul makdis to the questioners (hadith ref required)</li>
			   
			   
			   </ul>
			   
			   
			   </p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>621 Akaba</h2>
               <p>
			   
			   <ul>
			   <li>1st Pledge on 621</li>
			   <li>2nd Pledge on 622</li>
			   
			   
			   
			   
			   </ul>
			   
			   </p>
            </div>
         </div>
         
         <div class="container left">
            <div class="content">
               <h2>622 Hijrah</h2>
               <p>
               <ul>
                  <li>Making of Masjid Al Quba and Masjid Al Nabbi</li>
                  <li>Treaty with Jews in Madina</li>
                  <li>Conversion of Salman al Farsi</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>623 Change of Qibla</h2>
               <p>
               <ul>
                  <li>First Ramadan</li>
                  <li>Zakat is obligated</li>
                  <li>Death of Prophet (pbuh)'s daughter Rukaya (Ra)</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>624 Badar</h2>
               <p>Age 54</p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>625 Wuhud</h2>
               <p>Age 55</p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>626 Abu Hurayira (Ra) joins</h2>
               <p>
               <ul>
                  <li>Age 56</li>
                  <li>Alcohol is made Haram</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>Battle of Ahzab</h2>
               <p>...</p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>628 Poisoning of the Prophet (pbuh)</h2>
               <p>Age 59</p>
            </div>
         </div>
         
         <div class="container left">
            <div class="content">
               <h2>629 Openning of Makkah</h2>
               <p>
               <ul>
                  <li>Khaild Ibn Walid (Ra) Joins in</li>
                  <li>Battle of Mutah</li>
                  <li>Death of Prophet (pbuh)'s daughter Zaynaab (Ra)</li>
                  <li>Seige of Taif</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>630 Tabuk, the last Gazwa</h2>
               <p>
               <ul>
                  <li>Death of Prophet (pbuh)'s daughter Umm Kulthum (Ra)</li>
                  <li>Tabuk</li>
                  <li>Age 61</li>
                  <li>...</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>631 Hajj by Abu Bakar (Ra)</h2>
               <p>
               <ul>
                  <li>Ali (Ra) goes to Yemen</li>
                  <li>...</li>
                  <li>...</li>
                  <li>...</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container right">
            <div class="content">
               <h2>632 Last Hajj</h2>
               <p>
               <ul>
                  <li>Muad ibn Jabal and Abu Musa Al Ashaari sent to Yemen</li>
                  <li>Prophet (pbuh) falls ill</li>
                  <li>Death of the Prophet pbuh</li>
                  <li>Death of Fatimah (Ra)</li>
               </ul>
               </p>
            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>heading</h2>
               <p>
               <ul>
                  <li>...</li>
                  <li>...</li>
                  <li>...</li>
                  <li>...</li>
               </ul>
               </p>
            </div>
         </div>
         
         
      </div>
   </body>
</html>
