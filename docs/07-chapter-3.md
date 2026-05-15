# **Chapter III: Requirements Specification**
## **3.1. User Stories**

# **Report Version Log**


<table>
    <thead>
        <tr>
            <th style="width: 8%">Epic/Story ID</th>
            <th style="width: 15%">Title</th>
            <th style="width: 30%">Description</th>
            <th style="width: 37%">Acceptance Criteria</th>
            <th style="width: 10%">Related to (Epic ID)</th>
        </tr>
    </thead>
    <tbody>
        <!-- EPIC 1 - BOTH -->
        <tr>
            <td class="epic-id" style="text-align:center">EP01</td>
            <td style="text-align:center">Digital boarding record</td>
            <td>As an <strong>independent driver or company administrator</strong>, I want to quickly record which students board or are absent at each stop, to avoid errors and optimize the route.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver has arrived at a scheduled stop, <strong>When</strong> the student boards the vehicle, <strong>Then</strong> the system allows recording the "boarding" event with a timestamp.</li>
                    <li><strong>Given</strong> that the driver is at a stop and a student does not show up, <strong>When</strong> 2 minutes pass without registration, <strong>Then</strong> the system automatically notifies the parent about the absence.</li>
                    <li><strong>Given</strong> that the driver is operating without an internet connection, <strong>When</strong> recording boardings, <strong>Then</strong> the system stores events locally and synchronizes them when connectivity is restored.</li>
                    <li><strong>Given</strong> that a boarding is recorded, <strong>When</strong> the event is persisted, <strong>Then</strong> the system sends a push notification to the student's parent.</li>
                </ul>
            </td>
            <td style="text-align:center">-</td>
        </tr>
        <!-- EPIC 2 - BOTH -->
        <tr>
            <td class="epic-id" style="text-align:center">EP02</td>
            <td style="text-align:center">Route management</td>
            <td>As an <strong>independent driver or company administrator</strong>, I want to view and follow an organized route with defined stops, to reduce waiting times and fuel consumption.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver has started their shift, <strong>When</strong> accessing the day's route, <strong>Then</strong> the system shows the sequential order of stops with estimated arrival times.</li>
                    <li><strong>Given</strong> that a delay occurs at a stop, <strong>When</strong> the system detects the delay, <strong>Then</strong> it automatically recalculates estimated times for subsequent stops.</li>
                    <li><strong>Given</strong> that the driver has registered an absence, <strong>When</strong> the stop corresponds to that student, <strong>Then</strong> the system automatically skips the stop and reorders the route.</li>
                    <li><strong>Given</strong> that the driver wants to save fuel, <strong>When</strong> the system detects a more efficient alternative, <strong>Then</strong> it suggests the optimal route considering real-time traffic.</li>
                </ul>
            </td>
            <td style="text-align:center">-</td>
        </tr>
        <!-- EPIC 3 - BOTH -->
        <tr>
            <td class="epic-id" style="text-align:center">EP03</td>
            <td style="text-align:center">Incident logging</td>
            <td>As an <strong>independent driver or company administrator</strong>, I want to record events such as delays, absences, or route changes, to maintain service traceability.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that an incident occurs on the route, <strong>When</strong> the driver selects the incident type (delay, accident, route change), <strong>Then</strong> the system records the event with location and timestamp.</li>
                    <li><strong>Given</strong> that an incident is recorded, <strong>When</strong> the incident affects the estimated arrival time, <strong>Then</strong> the system automatically notifies affected parents.</li>
                    <li><strong>Given</strong> that the driver needs to document an incident, <strong>When</strong> attaching evidence (photo, audio, text), <strong>Then</strong> the system saves the attachment associated with the event.</li>
                    <li><strong>Given</strong> that the incident is closed, <strong>When</strong> the administrator or driver checks the history, <strong>Then</strong> the complete event timeline is displayed.</li>
                </ul>
            </td>
            <td style="text-align:center">-</td>
        </tr>
        <!-- EPIC 4 - COMPANY ONLY -->
        <tr>
            <td class="epic-id" style="text-align:center">EP04</td>
            <td style="text-align:center">Real-time fleet monitoring</td>
            <td>As a <strong>school mobility company administrator</strong>, I want to view all my vehicles in real time, to supervise route compliance and manage incidents.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the administrator accesses the dashboard, <strong>When</strong> selecting the fleet view, <strong>Then</strong> the system shows a map with the current location of all active units in the company.</li>
                    <li><strong>Given</strong> that a unit deviates from its established route, <strong>When</strong> the deviation exceeds a configurable threshold, <strong>Then</strong> the system generates an alert on the administrator's dashboard.</li>
                    <li><strong>Given</strong> that the administrator selects a specific unit, <strong>When</strong> viewing its details, <strong>Then</strong> the route traveled, stops made, and current status are displayed.</li>
                    <li><strong>Given</strong> that an emergency occurs in a unit, <strong>When</strong> the driver reports the emergency, <strong>Then</strong> the system highlights the unit on the dashboard with a visual alert indicator.</li>
                    <li><strong>Given</strong> that a unit has not sent a location for more than 5 minutes, <strong>When</strong> monitoring is running, <strong>Then</strong> the system generates a "Unit without signal" alert.</li>
                </ul>
            </td>
            <td style="text-align:center">-</td>
        </tr>
        <!-- EPIC 5A - INDEPENDENT DRIVER ONLY (Personal reports) -->
        <tr>
            <td class="epic-id" style="text-align:center">EP05A</td>
            <td style="text-align:center">Personal trip reports</td>
            <td>As an <strong>independent driver</strong>, I want to access my trip history, punctuality, and incidents, to evaluate my performance and improve my reputation.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver accesses their profile, <strong>When</strong> selecting "My history", <strong>Then</strong> the system shows the list of trips made in the last 30 days with dates and times.</li>
                    <li><strong>Given</strong> that the driver wants to know their punctuality, <strong>When</strong> checking their performance report, <strong>Then</strong> the system shows the percentage of on-time arrivals per stop.</li>
                    <li><strong>Given</strong> that the driver has had incidents, <strong>When</strong> checking the record, <strong>Then</strong> they see the list of recorded events with their resolutions.</li>
                    <li><strong>Given</strong> that the driver wants to share their reputation, <strong>When</strong> generating a summary, <strong>Then</strong> the system allows exporting a simple report (PDF) with their metrics.</li>
                </ul>
            </td>
            <td style="text-align:center">-</td>
        </tr>
        <!-- EPIC 5B - COMPANY ONLY (Management reports) -->
        <tr>
            <td class="epic-id" style="text-align:center">EP05B</td>
            <td style="text-align:center">Fleet management reports</td>
            <td>As a <strong>school mobility company administrator</strong>, I want to generate consolidated reports for the entire fleet (punctuality, attendance, fuel, billing), to evaluate the service and make decisions.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the administrator needs a punctuality report by driver, <strong>When</strong> selecting a date range, <strong>Then</strong> the system generates a report with the percentage of on-time arrivals per unit.</li>
                    <li><strong>Given</strong> that the administrator requires the monthly attendance consolidated report, <strong>When</strong> selecting the month and route, <strong>Then</strong> the system exports an Excel file with service days per student (useful for billing).</li>
                    <li><strong>Given</strong> that the administrator wants to evaluate fuel consumption, <strong>When</strong> checking the efficiency report, <strong>Then</strong> the system shows kilometers traveled vs. engine-on time per unit.</li>
                    <li><strong>Given</strong> that the administrator needs an incident report, <strong>When</strong> filtering by incident type and period, <strong>Then</strong> the system presents a table with dates, drivers, and descriptions.</li>
                    <li><strong>Given</strong> that the administrator must justify service quality to a school, <strong>When</strong> requesting an executive report, <strong>Then</strong> the system generates a consolidated PDF with key fleet indicators.</li>
                </ul>
            </td>
            <td style="text-align:center">-</td>
        </tr>
        <!-- USER STORY 01 - Record student boarding -->
        <tr>
            <td class="user-story-id" style="text-align:center">US01</td>
            <td style="text-align:center">Record student boarding</td>
            <td>As a <strong>driver</strong>, I want to record the moment a student boards the vehicle at each stop, to maintain a digital attendance record.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver has arrived at a scheduled stop and the student is present, <strong>When</strong> the driver selects the student from the list, <strong>Then</strong> the system records the event with a timestamp and location.</li>
                    <li><strong>Given</strong> that the boarding registration is successful, <strong>When</strong> the action is completed, <strong>Then</strong> the system sends a push notification to the student's parent with the message "Your child has boarded the bus."</li>
                    <li><strong>Given</strong> that the driver is operating without an internet connection, <strong>When</strong> recording a boarding, <strong>Then</strong> the system stores the event locally and automatically synchronizes it when connectivity is restored.</li>
                </ul>
            </td>
            <td style="text-align:center">EP01</td>
        </tr>
        <!-- USER STORY 02 - Automatic absence notification -->
        <tr>
            <td class="user-story-id" style="text-align:center">US02</td>
            <td style="text-align:center">Automatic absence notification</td>
            <td>As a <strong>driver</strong>, I want the system to automatically detect when a student does not show up at their stop, so I don't have to wait longer than necessary or manually call the parent.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver has arrived at a scheduled stop, <strong>When</strong> 2 minutes pass without the student's boarding being recorded, <strong>Then</strong> the system sends a notification to the parent informing them of the absence.</li>
                    <li><strong>Given</strong> that the absence is notified, <strong>When</strong> the parent responds that the student will not attend, <strong>Then</strong> the system automatically skips the stop and continues to the next one.</li>
                    <li><strong>Given</strong> that the absence is notified but the student shows up after the time limit, <strong>When</strong> the driver records the late boarding, <strong>Then</strong> the system records the event with a "student delay" mark.</li>
                </ul>
            </td>
            <td style="text-align:center">EP01</td>
        </tr>
        <!-- USER STORY 03 - View optimized route -->
        <tr>
            <td class="user-story-id" style="text-align:center">US03</td>
            <td style="text-align:center">View optimized daily route</td>
            <td>As a <strong>driver</strong>, I want to view the day's route with the order of stops and estimated times, to reduce waiting times and fuel consumption.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver has started their shift, <strong>When</strong> accessing the route screen, <strong>Then</strong> the system shows the sequential order of stops with the address and estimated arrival time for each.</li>
                    <li><strong>Given</strong> that the driver follows the suggested route, <strong>When</strong> completing a stop, <strong>Then</strong> the system automatically updates the view, showing the next stop as the current destination.</li>
                    <li><strong>Given</strong> that the driver deviates from the suggested route, <strong>When</strong> the system detects the deviation, <strong>Then</strong> it recalculates the remaining route and updates the estimated times.</li>
                </ul>
            </td>
            <td style="text-align:center">EP02</td>
        </tr>
        <!-- USER STORY 04 - Reorder route due to absence -->
        <tr>
            <td class="user-story-id" style="text-align:center">US04</td>
            <td style="text-align:center">Reorder route due to absence</td>
            <td>As a <strong>driver</strong>, I want the route to be automatically reordered when a student is absent, so I don't waste time passing by an empty stop.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that a student's absence at their stop has been confirmed, <strong>When</strong> the system receives the confirmation, <strong>Then</strong> it skips that stop from the active route and reorders the following ones.</li>
                    <li><strong>Given</strong> that the route has been reordered, <strong>When</strong> the driver views the updated route, <strong>Then</strong> the estimated arrival times have been recalculated for all remaining stops.</li>
                    <li><strong>Given</strong> that the absence was recorded by the parent before the route started, <strong>When</strong> the driver starts the shift, <strong>Then</strong> the absent student's stop does not appear on the day's route.</li>
                </ul>
            </td>
            <td style="text-align:center">EP02</td>
        </tr>
        <!-- USER STORY 05 - Record incident on route -->
        <tr>
            <td class="user-story-id" style="text-align:center">US05</td>
            <td style="text-align:center">Record incident on route</td>
            <td>As a <strong>driver</strong>, I want to record any incident that occurs during the trip (delay, accident, route change), to maintain service traceability.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that an incident occurs during the trip, <strong>When</strong> the driver selects the incident type (delay, accident, detour, medical emergency), <strong>Then</strong> the system records the event with location, timestamp, and vehicle data.</li>
                    <li><strong>Given</strong> that the driver needs to document the incident, <strong>When</strong> attaching a photo or text note, <strong>Then</strong> the system saves the evidence associated with the event.</li>
                    <li><strong>Given</strong> that the incident affects arrival times, <strong>When</strong> the driver records it, <strong>Then</strong> the system recalculates estimated times and notifies affected parents.</li>
                </ul>
            </td>
            <td style="text-align:center">EP03</td>
        </tr>
        <!-- USER STORY 06 - Notify parents due to incident (automatic) -->
        <tr>
            <td class="user-story-id" style="text-align:center">US06</td>
            <td style="text-align:center">Notify parents due to incident</td>
            <td>As a <strong>system</strong>, I want to automatically notify parents when an incident that affects their children's route is recorded, to keep them informed without manual intervention from the driver.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that an incident affecting estimated times is recorded, <strong>When</strong> the system calculates the new arrival time, <strong>Then</strong> it sends a push notification to the parents of affected students with the message "The bus will be delayed by X minutes."</li>
                    <li><strong>Given</strong> that a serious incident (accident, emergency) is recorded, <strong>When</strong> the driver marks the event as critical, <strong>Then</strong> the system immediately notifies the company administrator and sends a priority alert to parents.</li>
                    <li><strong>Given</strong> that the incident is resolved, <strong>When</strong> the driver confirms the service has returned to normal, <strong>Then</strong> the system sends a notification "Incident resolved - service continues as normal."</li>
                </ul>
            </td>
            <td style="text-align:center">EP03</td>
        </tr>
        <!-- USER STORY 07 - View complete fleet on map (Company) -->
        <tr>
            <td class="user-story-id" style="text-align:center">US07</td>
            <td style="text-align:center">View complete fleet on map</td>
            <td>As a <strong>school mobility company administrator</strong>, I want to view all my active vehicles on a map in real time, to supervise route compliance without relying on phone calls.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the administrator accesses the company dashboard, <strong>When</strong> selecting the fleet view, <strong>Then</strong> the system shows a map with the current location of all active vehicles, identified by number or driver name.</li>
                    <li><strong>Given</strong> that the administrator selects a specific vehicle on the map, <strong>When</strong> clicking on it, <strong>Then</strong> a panel displays the route details, stops made, next destination, and current status.</li>
                    <li><strong>Given</strong> that a vehicle has emergency mode activated, <strong>When</strong> the administrator views the map, <strong>Then</strong> that vehicle is highlighted with a distinctive alert icon or color.</li>
                </ul>
            </td>
            <td style="text-align:center">EP04</td>
        </tr>
        <!-- USER STORY 08 - Alert for route deviation -->
        <tr>
            <td class="user-story-id" style="text-align:center">US08</td>
            <td style="text-align:center">Receive alert for route deviation</td>
            <td>As a <strong>school mobility company administrator</strong>, I want to receive an alert when a vehicle significantly deviates from its established route, so I can act quickly in case of possible incidents.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that an active vehicle has a defined scheduled route, <strong>When</strong> its location deviates more than 500 meters from the planned route, <strong>Then</strong> the system generates an alert on the administrator's dashboard.</li>
                    <li><strong>Given</strong> that a deviation alert is generated, <strong>When</strong> the administrator clicks on the alert, <strong>Then</strong> the system shows the vehicle's current location and the scheduled route for comparison.</li>
                    <li><strong>Given</strong> that the deviation was authorized (e.g., due to road closure), <strong>When</strong> the driver previously recorded a planned detour, <strong>Then</strong> the system does not generate an alert for that specific deviation.</li>
                </ul>
            </td>
            <td style="text-align:center">EP04</td>
        </tr>
        <!-- USER STORY 09 - Personal trip history (Driver) -->
        <tr>
            <td class="user-story-id" style="text-align:center">US09</td>
            <td style="text-align:center">View personal trip history</td>
            <td>As an <strong>independent driver</strong>, I want to access my trip history, punctuality, and recorded incidents, to evaluate my performance and demonstrate my reliability to parents.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the driver accesses their profile in the app, <strong>When</strong> selecting "My history", <strong>Then</strong> the system shows a list of trips made in the last 30 days with date, start and end time.</li>
                    <li><strong>Given</strong> that the driver checks a specific day, <strong>When</strong> selecting a date, <strong>Then</strong> the system shows the route details: stops, actual vs. scheduled times, and recorded incidents.</li>
                    <li><strong>Given</strong> that the driver wants to share their history with a parent, <strong>When</strong> requesting to export their report, <strong>Then</strong> the system generates a summarized PDF with their punctuality metrics and number of incidents.</li>
                </ul>
            </td>
            <td style="text-align:center">EP05A</td>
        </tr>
        <!-- USER STORY 10 - Export monthly attendance report (Company) -->
        <tr>
            <td class="user-story-id" style="text-align:center">US10</td>
            <td style="text-align:center">Export monthly attendance report</td>
            <td>As a <strong>school mobility company administrator</strong>, I want to export a monthly attendance consolidated report per student, to streamline the billing process for parents without manual errors.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the administrator needs to bill per student, <strong>When</strong> selecting a month and a route, <strong>Then</strong> the system generates an Excel file with the list of students and the days of the month they actually used the service.</li>
                    <li><strong>Given</strong> that the report has been generated, <strong>When</strong> the administrator downloads it, <strong>Then</strong> the file contains columns: student name, grade, pickup address, total days served, justified and unjustified absences.</li>
                    <li><strong>Given</strong> that a student had absences recorded by the driver, <strong>When</strong> the report is generated, <strong>Then</strong> those absences appear marked with the type (justified or unjustified) as reported by the parent.</li>
                </ul>
            </td>
            <td style="text-align:center">EP05B</td>
        </tr>
        <!-- USER STORY 11 - Generate punctuality report per unit -->
        <tr>
            <td class="user-story-id" style="text-align:center">US11</td>
            <td style="text-align:center">Generate punctuality report per unit</td>
            <td>As a <strong>school mobility company administrator</strong>, I want to generate a punctuality report per driver/unit, to evaluate their performance and make improvement or incentive decisions.</td>
            <td class="acceptance-criteria">
                <ul>
                    <li><strong>Given</strong> that the administrator selects a date range, <strong>When</strong> requesting the punctuality report, <strong>Then</strong> the system generates a table with each unit, their percentage of on-time arrivals per stop, and the average delay in minutes.</li>
                    <li><strong>Given</strong> that the report has been generated, <strong>When</strong> the administrator selects a specific unit, <strong>Then</strong> the system shows the day-by-day details with scheduled vs. actual times.</li>
                    <li><strong>Given</strong> that the administrator needs to present the report to a school, <strong>When</strong> requesting to export as PDF, <strong>Then</strong> the system generates a professional document with weekly punctuality charts.</li>
                </ul>
            </td>
            <td style="text-align:center">EP05B</td>
        </tr>
          <tr>
    <td style="text-align: center;">US12</td>
    <td style="text-align: center;">View student list by route</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to see the list of students assigned to my route, so I know whom to pick up.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has logged into the app, <strong>When</strong> accessing the day's route section, <strong>Then</strong> the system presents the list of students ordered by stop sequence.</li>
            <li><strong>Given</strong> that the student list is visible, <strong>When</strong> the driver checks a specific student, <strong>Then</strong> the system shows their full name and pickup address.</li>
            <li><strong>Given</strong> that there are students assigned to different routes, <strong>When</strong> the driver views their list, <strong>Then</strong> the system filters and shows only the students assigned to the driver's active route.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
    <tr>
    <td style="text-align: center;">US13</td>
    <td style="text-align: center;">View students by stop</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to see which students correspond to each stop, to organize the pickup.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has selected an active route, <strong>When</strong> accessing the list of stops, <strong>Then</strong> the system groups students by each scheduled stop.</li>
            <li><strong>Given</strong> that the driver is at a specific stop, <strong>When</strong> checking the list, <strong>Then</strong> the system identifies the current stop with a distinct visual indicator.</li>
            <li><strong>Given</strong> that the driver needs to review other stops, <strong>When</strong> navigating between them, <strong>Then</strong> the system allows switching from one stop to another without losing route context.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
    <tr>
    <td style="text-align: center;">US14</td>
    <td style="text-align: center;">Record boarding</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to quickly mark when a student gets on, to keep track of the ride.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver is at a stop and the student boards the vehicle, <strong>When</strong> the driver performs the recording action, <strong>Then</strong> the system changes the student's status to "boarded" in the list.</li>
            <li><strong>Given</strong> that boarding has been recorded, <strong>When</strong> the driver continues with the route, <strong>Then</strong> the system automatically saves the event with timestamp and location.</li>
            <li><strong>Given</strong> that the recording is successful, <strong>When</strong> the driver checks the updated list, <strong>Then</strong> the student appears as already boarded and no further action is required.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
    <tr>
    <td style="text-align: center;">US15</td>
    <td style="text-align: center;">Record absence</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to mark when a student does not get on, to avoid unnecessary waiting.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has arrived at a scheduled stop and the student does not show up, <strong>When</strong> the driver selects the absence option, <strong>Then</strong> the system records the student as "absent" at that stop.</li>
            <li><strong>Given</strong> that the driver records an absence, <strong>When</strong> the system prompts, <strong>Then</strong> the driver can optionally record the reason for the absence.</li>
            <li><strong>Given</strong> that an absence is recorded, <strong>When</strong> the event is persisted, <strong>Then</strong> the information is updated in real time in the system and available to the administrator or parents.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
    <tr>
    <td style="text-align: center;">US16</td>
    <td style="text-align: center;">Quick status editing</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to correct a student's status in case of error, to maintain accurate information.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that a student has an erroneously recorded status (boarding or absence), <strong>When</strong> the driver selects the edit option, <strong>Then</strong> the system allows changing the status to the correct value.</li>
            <li><strong>Given</strong> that a status correction is made, <strong>When</strong> the change is saved, <strong>Then</strong> the system records the latest update with a new timestamp and maintains traceability of the change.</li>
            <li><strong>Given</strong> that the driver needs to correct a status, <strong>When</strong> accessing the edit, <strong>Then</strong> the system allows completing the correction without requiring multiple steps or additional screens.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
  <tr>
    <td style="text-align: center;">US17</td>
    <td style="text-align: center;">Offline functionality</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to be able to record boardings without an internet connection, so I don't depend on signal.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver's device has no internet connection, <strong>When</strong> the driver records a boarding or absence, <strong>Then</strong> the system stores the event locally on the device.</li>
            <li><strong>Given</strong> that there are pending events to synchronize, <strong>When</strong> the device regains internet connection, <strong>Then</strong> the system automatically sends all stored events to the server.</li>
            <li><strong>Given</strong> that synchronization is completed, <strong>When</strong> the system verifies the transmitted events, <strong>Then</strong> no information recorded during offline mode is lost or duplicated.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
  <tr>
    <td style="text-align: center;">US18</td>
    <td style="text-align: center;">Quick visual confirmation</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to quickly identify who has already gotten on and who hasn't, to make quick decisions.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver views the list of students at a stop, <strong>When</strong> a student has the status "boarded", <strong>Then</strong> the system visually differentiates them from those with pending status.</li>
            <li><strong>Given</strong> that the driver is on the move, <strong>When</strong> checking the student list, <strong>Then</strong> the system presents the information in a readable way without requiring complex interactions.</li>
            <li><strong>Given</strong> that the driver needs to know the general status of the stop, <strong>When</strong> reviewing the list, <strong>Then</strong> the system allows them to see at a glance how many students have boarded and how many are missing.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP01</td>
   </>
    <tr>
    <td style="text-align: center;">US19</td>
    <td style="text-align: center;">View assigned route</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to view the assigned route for the day, to know the order of travel.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has started their work shift, <strong>When</strong> accessing the route section, <strong>Then</strong> the system presents the assigned route for the current day.</li>
            <li><strong>Given</strong> that the day's route is visible, <strong>When</strong> the driver checks it, <strong>Then</strong> the system shows the complete list of stops in the sequential order of the journey.</li>
            <li><strong>Given</strong> that there are multiple drivers in the same company, <strong>When</strong> a driver checks their route, <strong>Then</strong> the system shows only the route assigned to that specific driver.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US20</td>
    <td style="text-align: center;">View stops on map</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to see the stops on my route on a map, to easily locate myself during the journey.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has selected their active route, <strong>When</strong> accessing the map view, <strong>Then</strong> the system shows all route stops as geolocated points.</li>
            <li><strong>Given</strong> that the map is visible, <strong>When</strong> the driver moves during the journey, <strong>Then</strong> the system shows the current vehicle location on the map.</li>
            <li><strong>Given</strong> that stops are represented on the map, <strong>When</strong> the driver views them, <strong>Then</strong> each stop is clearly differentiated (e.g., completed vs. pending stops).</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US21</td>
    <td style="text-align: center;">Navigation between stops</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to receive directions to reach each stop, to optimize my journey.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has completed a stop, <strong>When</strong> the system detects completion, <strong>Then</strong> it automatically selects the next stop as the next destination.</li>
            <li><strong>Given</strong> that the next stop is selected, <strong>When</strong> the driver needs guidance, <strong>Then</strong> the system provides navigation directions to reach that stop.</li>
            <li><strong>Given</strong> that the driver needs to change the navigation order, <strong>When</strong> manually selecting another stop, <strong>Then</strong> the system updates the directions to the newly selected stop.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US22</td>
    <td style="text-align: center;">Mark stop as completed</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to mark a stop as completed, to advance along my route in an orderly manner.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has completed the actions at a stop (boardings and absences), <strong>When</strong> the driver performs the action to finish the stop, <strong>Then</strong> the system changes the stop's status to "completed".</li>
            <li><strong>Given</strong> that a stop has been marked as completed, <strong>When</strong> the driver views the stop list, <strong>Then</strong> the completed stop is visually differentiated from pending stops.</li>
            <li><strong>Given</strong> that the current stop is marked as completed, <strong>When</strong> the system records the event, <strong>Then</strong> it automatically advances to the next stop on the route.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US23</td>
    <td style="text-align: center;">Basic route reordering</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to adjust the order of stops in case of unforeseen events, to adapt to changes in the journey.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that an unforeseen event occurs requiring a change in the order of stops, <strong>When</strong> the driver modifies the stop sequence, <strong>Then</strong> the system allows reordering the list according to the new priority.</li>
            <li><strong>Given</strong> that the driver has reordered the stops, <strong>When</strong> confirming the changes, <strong>Then</strong> the system updates the active route in real time with the new order.</li>
            <li><strong>Given</strong> that the route has been reordered, <strong>When</strong> the driver checks student records, <strong>Then</strong> the boarding and absence data remain correctly associated with each student.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US24</td>
    <td style="text-align: center;">View route status</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to see my route progress, to know how much is left to complete.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has an active route, <strong>When</strong> accessing the progress view, <strong>Then</strong> the system shows the number or percentage of stops completed out of the total.</li>
            <li><strong>Given</strong> that the driver views the route status, <strong>When</strong> checking the stop list, <strong>Then</strong> the system clearly differentiates between completed stops and pending stops.</li>
            <li><strong>Given</strong> that the driver progresses along their journey, <strong>When</strong> completing a new stop, <strong>Then</strong> the system updates the progress status in real time.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US25</td>
    <td style="text-align: center;">Offline route functionality</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to access my route without an internet connection, so I don't depend on signal.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has an internet connection at the start of the shift, <strong>When</strong> the system downloads the assigned route, <strong>Then</strong> the route data is stored locally on the device.</li>
            <li><strong>Given</strong> that the route is stored locally, <strong>When</strong> the device has no internet connection, <strong>Then</strong> the driver can view the route and its stops without interruptions.</li>
            <li><strong>Given</strong> that the driver makes changes to the route (reordering, statuses) without connection, <strong>When</strong> the device regains connection, <strong>Then</strong> the system automatically synchronizes all pending changes with the server.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP02</td>
   </>
  <tr>
    <td style="text-align: center;">US26</td>
    <td style="text-align: center;">Quick incident logging</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to record an incident in a few steps, so I don't get distracted during the journey.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that an unexpected event occurs during the journey, <strong>When</strong> the driver needs to report it, <strong>Then</strong> the system allows starting the incident log with an accessible action.</li>
            <li><strong>Given</strong> that the driver has started logging an incident, <strong>When</strong> selecting the event type, <strong>Then</strong> the system allows completing the selection in a maximum of two interactions.</li>
            <li><strong>Given</strong> that the driver needs to log the incident, <strong>When</strong> completing the log, <strong>Then</strong> the system does not require the driver to write text to save the event.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US28</td>
    <td style="text-align: center;">Select incident type</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to choose the incident type, to correctly classify the event.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver is logging an incident, <strong>When</strong> accessing the type selection, <strong>Then</strong> the system presents a predefined list of available incident types.</li>
            <li><strong>Given</strong> that the list of incident types is visible, <strong>When</strong> the driver reviews it, <strong>Then</strong> each option is worded clearly and understandably for their context.</li>
            <li><strong>Given</strong> that the driver needs to classify the incident, <strong>When</strong> selecting a type, <strong>Then</strong> the system allows choosing only one main option per event.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US29</td>
    <td style="text-align: center;">Record optional detail</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to add an optional comment, to provide more context if necessary.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver is logging an incident, <strong>When</strong> they wish to add additional information, <strong>Then</strong> the system has a field for optionally entering text.</li>
            <li><strong>Given</strong> that the driver has no additional information to add, <strong>When</strong> skipping the comment field, <strong>Then</strong> the system allows completing the log without blocking the action.</li>
            <li><strong>Given</strong> that the driver enters a comment, <strong>When</strong> the incident is saved, <strong>Then</strong> the system stores the comment along with the rest of the event data.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US30</td>
    <td style="text-align: center;">Associate incident with stop or student</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to link the incident to a stop or student, for greater precision in the log.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver is logging an incident, <strong>When</strong> the incident is related to a specific point on the journey, <strong>Then</strong> the system allows selecting the associated stop or student.</li>
            <li><strong>Given</strong> that the driver links the incident to a stop or student, <strong>When</strong> confirming the log, <strong>Then</strong> the system saves the association as part of the event.</li>
            <li><strong>Given</strong> that the incident is not related to a specific stop or student, <strong>When</strong> the driver completes the log, <strong>Then</strong> the system allows saving the incident without needing to make an association.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US31</td>
    <td style="text-align: center;">Automatic time and location logging</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want the system to automatically record the time and location, so I don't have to do it manually.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver logs an incident, <strong>When</strong> the event is created, <strong>Then</strong> the system automatically saves a timestamp with the date and time of registration.</li>
            <li><strong>Given</strong> that the driver logs an incident, <strong>When</strong> the device has GPS available, <strong>Then</strong> the system automatically captures and stores the geographic location of the event.</li>
            <li><strong>Given</strong> that the system records time and location, <strong>When</strong> the log is completed, <strong>Then</strong> no additional action is required from the driver to capture this data.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US32</td>
    <td style="text-align: center;">View incident history</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to see the logged incidents, to track the journey.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver needs to review the day's events, <strong>When</strong> accessing the incident history, <strong>Then</strong> the system presents a list of all incidents logged during the current shift.</li>
            <li><strong>Given</strong> that the incident list is visible, <strong>When</strong> the driver checks an event, <strong>Then</strong> the system shows the incident type, registration time, and current status.</li>
            <li><strong>Given</strong> that multiple incidents have been logged, <strong>When</strong> the driver views the list, <strong>Then</strong> the system presents them in chronological order (from newest to oldest or vice versa).</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US33</td>
    <td style="text-align: center;">Edit or correct incident</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to correct an incident in case of error, to maintain accurate information.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver identifies an error in a previously logged incident, <strong>When</strong> accessing the edit option, <strong>Then</strong> the system allows modifying the incident type and/or associated comment.</li>
            <li><strong>Given</strong> that the driver has made changes to an incident, <strong>When</strong> confirming the edit, <strong>Then</strong> the system correctly saves the new values.</li>
            <li><strong>Given</strong> that an incident is edited, <strong>When</strong> the driver checks the history, <strong>Then</strong> the system shows the updated information with the record of the last modification.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US34</td>
    <td style="text-align: center;">Offline incident functionality</td>
    <td style="text-align: center;">As a <strong>driver</strong>, I want to log incidents without connection, so I don't depend on the network.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver's device has no internet connection, <strong>When</strong> the driver logs an incident, <strong>Then</strong> the system stores the incident locally on the device.</li>
            <li><strong>Given</strong> that there are pending incidents to synchronize, <strong>When</strong> the device regains internet connection, <strong>Then</strong> the system automatically sends all stored incidents to the server.</li>
            <li><strong>Given</strong> that synchronization is completed, <strong>When</strong> the system verifies the transmitted data, <strong>Then</strong> no incident logged during offline mode is lost.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP03</td>
   </>
  <tr>
    <td style="text-align: center;">US35</td>
    <td style="text-align: center;">View vehicles on map</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to see all my vehicles on a real-time map, to monitor their location.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator accesses the monitoring dashboard, <strong>When</strong> selecting the map view, <strong>Then</strong> the system shows all active company vehicles geolocated on the map.</li>
            <li><strong>Given</strong> that the vehicles are represented on the map, <strong>When</strong> the administrator views them, <strong>Then</strong> each vehicle has a visible identifier (driver number or name).</li>
            <li><strong>Given</strong> that the vehicles move during the shift, <strong>When</strong> their location changes, <strong>Then</strong> the system automatically updates the positions on the map.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US36</td>
    <td style="text-align: center;">View vehicle details</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to select a vehicle and see its information, to know its current status.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator views the map with active vehicles, <strong>When</strong> selecting a specific vehicle, <strong>Then</strong> the system displays a panel with detailed information about that vehicle.</li>
            <li><strong>Given</strong> that the detail panel is visible, <strong>When</strong> the administrator checks the information, <strong>Then</strong> the system shows the driver's data, the assigned route, and the vehicle's current status.</li>
            <li><strong>Given</strong> that the vehicle's information has changed, <strong>When</strong> the administrator checks the details, <strong>Then</strong> the data presented is updated at the time of the query.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US37</td>
    <td style="text-align: center;">View vehicle statuses</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to identify the status of each vehicle, to quickly detect problems.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator views the map or vehicle list, <strong>When</strong> checking their status, <strong>Then</strong> the system shows the current status of each vehicle (on route, stopped, delayed).</li>
            <li><strong>Given</strong> that statuses are represented, <strong>When</strong> the administrator reviews them, <strong>Then</strong> each status is visually differentiated from the others (e.g., visual distinctive mark according to the status type).</li>
            <li><strong>Given</strong> that a vehicle's status changes during the shift, <strong>When</strong> the change occurs, <strong>Then</strong> the system updates the information in real time on the administrator's dashboard.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US38</td>
    <td style="text-align: center;">Filter units</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to filter vehicles by status or route, to focus on what is relevant.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator views the vehicle list or map, <strong>When</strong> applying a filter by status, <strong>Then</strong> the system shows only the vehicles that match the selected status.</li>
            <li><strong>Given</strong> that the administrator needs to filter by route, <strong>When</strong> selecting a specific route, <strong>Then</strong> the system shows only the vehicles assigned to that route.</li>
            <li><strong>Given</strong> that the administrator applies one or more filters, <strong>When</strong> confirming the selection, <strong>Then</strong> the view is automatically updated showing only the vehicles that meet the criteria.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US39</td>
    <td style="text-align: center;">Deviation alerts</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to receive alerts when a vehicle deviates from its route, to take timely action.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that an active vehicle has a defined scheduled route, <strong>When</strong> its location significantly deviates from the planned route, <strong>Then</strong> the system automatically detects the deviation.</li>
            <li><strong>Given</strong> that a deviation is detected, <strong>When</strong> the event occurs, <strong>Then</strong> the system generates a visible alert or notification for the administrator.</li>
            <li><strong>Given</strong> that a deviation alert is generated, <strong>When</strong> the administrator receives it, <strong>Then</strong> the alert clearly indicates which vehicle has the problem.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US40</td>
    <td style="text-align: center;">View real-time journey</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to see the journey each vehicle is making, to validate route compliance.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator selects an active vehicle, <strong>When</strong> accessing the journey view, <strong>Then</strong> the system shows the trajectory the vehicle has followed on the map.</li>
            <li><strong>Given</strong> that the trajectory is visible, <strong>When</strong> the vehicle advances during its journey, <strong>Then</strong> the system updates the trajectory on the map as it progresses.</li>
            <li><strong>Given</strong> that the administrator checks a vehicle's journey, <strong>When</strong> viewing it, <strong>Then</strong> the system allows identifying which part of the route has already been completed and what remains.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US41</td>
    <td style="text-align: center;">Recent location history</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to check a vehicle's recent locations, to analyze its behavior.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator selects a specific vehicle, <strong>When</strong> accessing the history section, <strong>Then</strong> the system shows the recent locations recorded for that vehicle.</li>
            <li><strong>Given</strong> that the location history is visible, <strong>When</strong> the administrator checks it, <strong>Then</strong> the locations are presented in chronological order.</li>
            <li><strong>Given</strong> that the administrator needs to review a vehicle's history, <strong>When</strong> on the vehicle details page, <strong>Then</strong> the system allows accessing the history from that same view.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US42</td>
    <td style="text-align: center;">Automatic data refresh</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want the information to refresh automatically, so I don't have to manually reload.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the administrator is viewing the monitoring dashboard, <strong>When</strong> a defined time interval elapses, <strong>Then</strong> the system automatically updates the displayed data.</li>
            <li><strong>Given</strong> that the data updates automatically, <strong>When</strong> the update occurs, <strong>Then</strong> the administrator does not need to perform any manual action to reload the information.</li>
            <li><strong>Given</strong> that an automatic update has been performed, <strong>When</strong> the administrator checks the information, <strong>Then</strong> the system indicates the time of the last update performed.</li>
            <li><strong>Given</strong> that the data updates in the background, <strong>When</strong> the update occurs, <strong>Then</strong> the administrator's navigation or interaction is not interrupted.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP04</td>
   </>
  <tr>
    <td style="text-align: center;">US43</td>
    <td style="text-align: center;">Generate journey report</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to generate reports of completed journeys, to analyze route compliance.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator needs a journey report, <strong>When</strong> selecting a date range, <strong>Then</strong> the system generates a report with the journeys completed in that period.</li>
            <li><strong>Given</strong> that the report has been generated, <strong>When</strong> the administrator checks it, <strong>Then</strong> the report includes the routes taken by each vehicle.</li>
            <li><strong>Given</strong> that the report is available, <strong>When</strong> the administrator views it, <strong>Then</strong> the information is presented on screen in a readable way.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
  <tr>
    <td style="text-align: center;">US44</td>
    <td style="text-align: center;">Generate performance report</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to view driver and vehicle performance metrics, to evaluate operational efficiency.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator requests a performance report, <strong>When</strong> the report is generated, <strong>Then</strong> the system shows key metrics such as travel times and stops completed.</li>
            <li><strong>Given</strong> that the performance report is visible, <strong>When</strong> the administrator checks it, <strong>Then</strong> the information is presented grouped by driver or by vehicle.</li>
            <li><strong>Given</strong> that the report contains metrics, <strong>When</strong> the administrator reviews them, <strong>Then</strong> the data is clear, understandable, and allows evaluating operational efficiency.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
  <tr>
    <td style="text-align: center;">US45</td>
    <td style="text-align: center;">Export reports</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to export reports, to share or analyze them externally.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator has generated a report, <strong>When</strong> selecting the export option, <strong>Then</strong> the system allows exporting the report in PDF or Excel format.</li>
            <li><strong>Given</strong> that the export is initiated, <strong>When</strong> the process completes, <strong>Then</strong> the file downloads quickly to the administrator's device.</li>
            <li><strong>Given</strong> that the administrator exports a report, <strong>When</strong> opening the downloaded file, <strong>Then</strong> the content includes all the information selected during report generation.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
  <tr>
    <td style="text-align: center;">US46</td>
    <td style="text-align: center;">Filter reports</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to apply filters to reports, to focus on specific information.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator is generating a report, <strong>When</strong> applying a filter by date range, <strong>Then</strong> the system shows only the information corresponding to that period.</li>
            <li><strong>Given</strong> that the administrator needs specific information, <strong>When</strong> applying a filter by driver or by vehicle, <strong>Then</strong> the system shows only the data associated with that driver or vehicle.</li>
            <li><strong>Given</strong> that the administrator applies one or more filters, <strong>When</strong> confirming the selection, <strong>Then</strong> the report information is automatically updated according to the applied filters.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
  <tr>
    <td style="text-align: center;">US47</td>
    <td style="text-align: center;">Include incidents in reports</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to include incidents in reports, to have complete service context.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator generates a report, <strong>When</strong> the report includes incidents, <strong>Then</strong> the system shows the incidents recorded in the selected period.</li>
            <li><strong>Given</strong> that incidents are visible in the report, <strong>When</strong> the administrator checks them, <strong>Then</strong> each incident is associated with the corresponding route or vehicle.</li>
            <li><strong>Given</strong> that the administrator exports the report, <strong>When</strong> the file is generated, <strong>Then</strong> the incidents are included in the exported report.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
  <tr>
    <td style="text-align: center;">US48</td>
    <td style="text-align: center;">General summary</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to see a general performance summary, to make quick decisions.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator accesses the reports dashboard, <strong>When</strong> viewing the general summary, <strong>Then</strong> the system shows summarized key operational performance indicators.</li>
            <li><strong>Given</strong> that the general summary is visible, <strong>When</strong> the administrator checks it, <strong>Then</strong> the presentation of indicators is simple, clear, and easy to understand.</li>
            <li><strong>Given</strong> that the administrator uses the summary for decision-making, <strong>When</strong> the data changes during the shift, <strong>Then</strong> the system periodically updates the indicators.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
  <tr>
    <td style="text-align: center;">US49</td>
    <td style="text-align: center;">Quick download of recent reports</td>
    <td style="text-align: center;">As a <strong>school mobility company administrator</strong>, I want to quickly access recent reports, to save time on frequent queries.</td>
    <td class="acceptance-criteria"><ul>
            <li><strong>Given</strong> that the administrator has previously generated reports, <strong>When</strong> accessing the recent reports section, <strong>Then</strong> the system presents a list of recently generated reports.</li>
            <li><strong>Given</strong> that the administrator views the list of recent reports, <strong>When</strong> selecting one of them, <strong>Then</strong> the system allows accessing the report with a single action.</li>
            <li><strong>Given</strong> that the administrator needs a report already generated previously, <strong>When</strong> accessing it from the recent list, <strong>Then</strong> there is no need to generate it again from scratch.</li>
        </ul></td>
    <td style="text-align: center;">EP05B</td>
   </>
    <tr>
    <td style="text-align: center;">US50</td>
    <td style="text-align: center;">View personal trip summary</td>
    <td style="text-align: center;">As an <strong>independent driver</strong>, I want to see a summary of my completed trips, to track my daily activity.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has completed one or more trips, <strong>When</strong> accessing their reports section, <strong>Then</strong> the system shows a summary of trips completed during the shift or selected period.</li>
            <li><strong>Given</strong> that the trip summary is visible, <strong>When</strong> the driver checks it, <strong>Then</strong> the system includes the number of trips, stops made, and times.</li>
            <li><strong>Given</strong> that the driver needs to review their activity, <strong>When</strong> accessing the summary, <strong>Then</strong> the information is clear and easy to understand.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP05A</td>
   </>
    <tr>
    <td style="text-align: center;">US51</td>
    <td style="text-align: center;">View personal punctuality metrics</td>
    <td style="text-align: center;">As an <strong>independent driver</strong>, I want to see my punctuality metrics, to evaluate my performance and improve my reputation.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has made trips in recent days, <strong>When</strong> accessing their punctuality metrics, <strong>Then</strong> the system shows the percentage of on-time arrivals per stop or per trip.</li>
            <li><strong>Given</strong> that the metrics are visible, <strong>When</strong> the driver checks them, <strong>Then</strong> the information is presented clearly and understandably.</li>
            <li><strong>Given</strong> that the driver wants to improve their reputation, <strong>When</strong> reviewing their metrics, <strong>Then</strong> they can identify days or stops where they had delays.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP05A</td>
   </>
    <tr>
    <td style="text-align: center;">US52</td>
    <td style="text-align: center;">Export personal trip history</td>
    <td style="text-align: center;">As an <strong>independent driver</strong>, I want to export my trip history, to share it with parents or companies that request references.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has selected a time period, <strong>When</strong> requesting to export their history, <strong>Then</strong> the system allows exporting the data in PDF format.</li>
            <li><strong>Given</strong> that the export is initiated, <strong>When</strong> the process completes, <strong>Then</strong> the downloaded file includes the trips made, dates, times, and punctuality.</li>
            <li><strong>Given</strong> that the driver needs to demonstrate their reliability, <strong>When</strong> sharing the exported report, <strong>Then</strong> the information is sufficient to validate their performance.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP05A</td>
   </>
    <tr>
    <td style="text-align: center;">US53</td>
    <td style="text-align: center;">View personal incident history</td>
    <td style="text-align: center;">As an <strong>independent driver</strong>, I want to see the incidents I have recorded, to have traceability of events that occurred during my services.</td>
    <td class="acceptance-criteria">
        <ul>
            <li><strong>Given</strong> that the driver has recorded incidents on past trips, <strong>When</strong> accessing their incident history, <strong>Then</strong> the system shows a list of recorded incidents.</li>
            <li><strong>Given</strong> that the incident list is visible, <strong>When</strong> the driver checks it, <strong>Then</strong> each incident includes the type, date, time, and location.</li>
            <li><strong>Given</strong> that the driver needs to justify an event to a parent or company, <strong>When</strong> checking the details of an incident, <strong>Then</strong> the information is sufficient to support their explanation.</li>
        </ul>
    </td>
    <td style="text-align: center;">EP05A</td>
  </tr>
    </tbody>
</table>


## **3.2. Impact Mapping**

![Impact Mapping](../assets/chapter-3/impact-mapping.jpg)

## **3.3. Product Backlog**

| Order | User Story Id | Title | Description | Story Points |
|-------|---------------|-------|-------------|--------------|
| 1 | US01 | Record student boarding | As a driver, I want to record the moment a student boards the vehicle at each stop, to maintain a digital attendance record. | 3 |
| 2 | US02 | Automatic absence notification | As a driver, I want the system to automatically detect when a student does not show up at their stop, so I don't have to wait longer than necessary or manually call the parent. | 3 |
| 3 | US14 | Record boarding | As a driver, I want to quickly mark when a student gets on, to keep track of the ride. | 2 |
| 4 | US15 | Record absence | As a driver, I want to mark when a student does not get on, to avoid unnecessary waiting. | 2 |
| 5 | US12 | View student list by route | As a driver, I want to see the list of students assigned to my route, so I know whom to pick up. | 2 |
| 6 | US13 | View students by stop | As a driver, I want to see which students correspond to each stop, to organize the pickup. | 2 |
| 7 | US18 | Quick visual confirmation | As a driver, I want to quickly identify who has already gotten on and who hasn't, to make quick decisions. | 1 |
| 8 | US16 | Quick status editing | As a driver, I want to correct a student's status in case of error, to maintain accurate information. | 2 |
| 9 | US17 | Offline functionality | As a driver, I want to be able to record boardings without an internet connection, so I don't depend on signal. | 5 |
| 10 | US03 | View optimized daily route | As a driver, I want to view the day's route with the order of stops and estimated times, to reduce waiting times and fuel consumption. | 3 |
| 11 | US19 | View assigned route | As a driver, I want to view the assigned route for the day, to know the order of travel. | 2 |
| 12 | US20 | View stops on map | As a driver, I want to see the stops on my route on a map, to easily locate myself during the journey. | 3 |
| 13 | US21 | Navigation between stops | As a driver, I want to receive directions to reach each stop, to optimize my journey. | 3 |
| 14 | US22 | Mark stop as completed | As a driver, I want to mark a stop as completed, to advance along my route in an orderly manner. | 1 |
| 15 | US24 | View route status | As a driver, I want to see my route progress, to know how much is left to complete. | 2 |
| 16 | US04 | Reorder route due to absence | As a driver, I want the route to be automatically reordered when a student is absent, so I don't waste time passing by an empty stop. | 3 |
| 17 | US23 | Basic route reordering | As a driver, I want to adjust the order of stops in case of unforeseen events, to adapt to changes in the journey. | 3 |
| 18 | US25 | Offline route functionality | As a driver, I want to access my route without an internet connection, so I don't depend on signal. | 5 |
| 19 | US05 | Record incident on route | As a driver, I want to record any incident that occurs during the trip (delay, accident, route change), to maintain service traceability. | 3 |
| 20 | US26 | Quick incident logging | As a driver, I want to record an incident in a few steps, so I don't get distracted during the journey. | 2 |
| 21 | US28 | Select incident type | As a driver, I want to choose the incident type, to correctly classify the event. | 2 |
| 22 | US29 | Record optional detail | As a driver, I want to add an optional comment, to provide more context if necessary. | 1 |
| 23 | US30 | Associate incident with stop or student | As a driver, I want to link the incident to a stop or student, for greater precision in the log. | 2 |
| 24 | US31 | Automatic time and location logging | As a driver, I want the system to automatically record the time and location, so I don't have to do it manually. | 2 |
| 25 | US32 | View incident history | As a driver, I want to see the logged incidents, to track the journey. | 2 |
| 26 | US33 | Edit or correct incident | As a driver, I want to correct an incident in case of error, to maintain accurate information. | 2 |
| 27 | US34 | Offline incident functionality | As a driver, I want to log incidents without connection, so I don't depend on the network. | 5 |
| 28 | US06 | Notify parents due to incident | As a system, I want to automatically notify parents when an incident that affects their children's route is recorded, to keep them informed without manual intervention from the driver. | 3 |
| 29 | US07 | View complete fleet on map | As a school mobility company administrator, I want to view all my active vehicles on a map in real time, to supervise route compliance without relying on phone calls. | 3 |
| 30 | US35 | View vehicles on map | As a school mobility company administrator, I want to see all my vehicles on a real-time map, to monitor their location. | 3 |
| 31 | US36 | View vehicle details | As a school mobility company administrator, I want to select a vehicle and see its information, to know its current status. | 2 |
| 32 | US37 | View vehicle statuses | As a school mobility company administrator, I want to identify the status of each vehicle, to quickly detect problems. | 2 |
| 33 | US38 | Filter units | As a school mobility company administrator, I want to filter vehicles by status or route, to focus on what is relevant. | 2 |
| 34 | US39 | Deviation alerts | As a school mobility company administrator, I want to receive alerts when a vehicle deviates from its route, to take timely action. | 3 |
| 35 | US08 | Receive alert for route deviation | As a school mobility company administrator, I want to receive an alert when a vehicle significantly deviates from its established route, so I can act quickly in case of possible incidents. | 3 |
| 36 | US40 | View real-time journey | As a school mobility company administrator, I want to see the journey each vehicle is making, to validate route compliance. | 3 |
| 37 | US41 | Recent location history | As a school mobility company administrator, I want to check a vehicle's recent locations, to analyze its behavior. | 2 |
| 38 | US42 | Automatic data refresh | As a school mobility company administrator, I want the information to refresh automatically, so I don't have to manually reload. | 3 |
| 39 | US09 | View personal trip history | As an independent driver, I want to access my trip history, punctuality, and recorded incidents, to evaluate my performance and demonstrate my reliability to parents. | 3 |
| 40 | US50 | View personal trip summary | As an independent driver, I want to see a summary of my completed trips, to track my daily activity. | 2 |
| 41 | US51 | View personal punctuality metrics | As an independent driver, I want to see my punctuality metrics, to evaluate my performance and improve my reputation. | 3 |
| 42 | US52 | Export personal trip history | As an independent driver, I want to export my trip history, to share it with parents or companies that request references. | 3 |
| 43 | US53 | View personal incident history | As an independent driver, I want to see the incidents I have recorded, to have traceability of events that occurred during my services. | 2 |
| 44 | US10 | Export monthly attendance report | As a school mobility company administrator, I want to export a monthly attendance consolidated report per student, to streamline the billing process for parents without manual errors. | 5 |
| 45 | US11 | Generate punctuality report per unit | As a school mobility company administrator, I want to generate a punctuality report per driver/unit, to evaluate their performance and make improvement or incentive decisions. | 5 |
| 46 | US43 | Generate journey report | As a school mobility company administrator, I want to generate reports of completed journeys, to analyze route compliance. | 3 |
| 47 | US44 | Generate performance report | As a school mobility company administrator, I want to view driver and vehicle performance metrics, to evaluate operational efficiency. | 5 |
| 48 | US45 | Export reports | As a school mobility company administrator, I want to export reports, to share or analyze them externally. | 3 |
| 49 | US46 | Filter reports | As a school mobility company administrator, I want to apply filters to reports, to focus on specific information. | 2 |
| 50 | US47 | Include incidents in reports | As a school mobility company administrator, I want to include incidents in reports, to have complete service context. | 2 |
| 51 | US48 | General summary | As a school mobility company administrator, I want to see a general performance summary, to make quick decisions. | 3 |
| 52 | US49 | Quick download of recent reports | As a school mobility company administrator, I want to quickly access recent reports, to save time on frequent queries. | 2 |