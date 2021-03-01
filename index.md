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
      <div class="timeline">
         <div class="container right">
            <div class="content">
               <h2>Prophet Ibrahim (As)</h2>
               <p>
               <ul>
                  <li>Breaks Idols</li>
                  <li>Father thorws him out of the home</li>
                  <li>Goes for in search of God</li>
                  <li>King throws Ibrahim (As) in fire</li>
                  <li>Ibrahim (As) says "HabunAllah owa ni maal owakeel", recorded in Quran</li>
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
                  <li>Angel visits and gives good news of son to Ibrahim (As)</li>
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
               <h2>Qusai Ibn Qalb</h2>
               <p>
               <ul>
                  <li>How he went to top of the chain</li>
                  <li>Uniting the Qurayesh</li>
                  <li>His sons</li>
                  <li>Duties and responsibilities of taking care of Hajjis</li>
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
               <h2>Haleema</h2>
               <p>
               <ul>
                  <li>Makkan's had a tradition of sending young kids to deserts for learning pure language and to be tough in the harsh environment</li>
                  <li>Haleema was one of the foster mothers who was looking for a baby to take care</li>
                  <li>None took Prophet pbuh as he pbuh was an orphan, except Haleema (Ra)</li>
                  <li>During his pbuh stay at Haleema (Ra) the incident with Angel Gibrael took place where he came and washed his (pbuh) heart as per the hadith. Narrated by Muslim (162)</li>
				  
               </ul>
               </p>



            </div>
         </div>
         <div class="container left">
            <div class="content">
               <h2>Losing Mother and Grandfather</h2>
               <p>
			   
			   Death of Mother Ameena and Abdul Muttalib
			   </p>
            </div>
         </div>
         
         <div class="container left">
            <div class="content">
               <h2>Before Marriage</h2>
               <p>as per "When the Moon Split" compilled by S R Mubarakpuri:
               <ul>
                  <li>Age 12 Prophet (pbuh) went to Syria with his (pbuh) uncle Abu Talib</li>
                  <li>A christian monk named as Bahira recognised Prophet (pbuh) as having sings of being a prophet</li>
                  <li>Bahira warned Abu talib to take the Prophet (pbuh) at a safe place in case the Bizentines finds out about him and kill him</li>
                  <li>Prophet pbuh participated Battle of Fijar at the age of 20 on the side of Qurayesh</li>
                  <li>Hilf ul Fudul was formed</li>
                  <li>Taking care of Goats for Makkans as a profession</li>
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
				  
				  <p>
				  <ul>
				  Over the nex few years, Prophet pbuh gets blessed with four daughters:
				  <li>Birth of first daugher Zainaab (Ra)</li>
                  <li>Birth of second daugher Ruqaiya (Ra)</li>
                  <li>Birth of third daugher Umm Kulthum (Ra)</li>
                  <li>Birth of fourth daugher Fatimah (Ra)</li>
				  </ul>
				  </p>
				  
				  
				  
				  
				  
               </ul>
               </p>
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
			   <li>Age 40 (39 years and some months)</li>
			   <li>Secret Preaching</li>
			   <li>Procecution of Muslims</li>
			   <li>614 Sumayia's death</li>
			   <li>615 First migration to Abisynia</li>
			   <li>615 Hamza (Ra) joins in</li>
			   	<li>616 Omar (Ra) joins in</li>
				
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
			   <li>Prayer was revealed</li>
			   <li>Last few verses of Surah Bakarah was revealed (verification required)</li>
			   <li>Firstly Prophet pbuh goes from Makkah to Jerujalem and from there to Heaven</li>
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

