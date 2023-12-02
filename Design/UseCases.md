# Use Cases
* UC1. (Corresponds to BR1, BR2) Reduce employee stress by administering stress reducing stimuli
   * We aim to reduce employee stress via the administration of stress reducing stimuli. This stimuli is most effective in VR format, thus employees of high stress demographics will utilize VR headsets to receive their stress reduction stimuli. The intended result is that employees will experience reduced stress during and after exposure to VR stress reduction stimuli. 
   * High Stress Employees
   * Program Flow:
      * Users access web app to request help with stress
      * Backend evaluates user data to select appropriate response
      * Response is provided via web app/VR device
* UC2. (Corresponds to BR2) Access visualized employees stress biometric data for analysis
   * Data analysts will want to be able to access both real time and recorded visualizations of employee stress biometric data. A live graph will be present, along with a recording of said graph as it evolves. A final chart will demonstrate how the graph changed over the duration of treatment/exposure. 
   * Data Analysts
   * Program Flow:
      * Participant data is collected via VR headset and stored in AWS backend
      * Analysts request data via web app
      * Data is retrieved from AWS backend, visualized, and displayed
* UC3. (Corresponds to BR1, BR2) Identify most common workplace stressors
   * The cumulative data collected and utilized by data analysts will allow the owner to determine the most common workplace stressors in each workplace that is analyzed. Recorded historic biometric data will play a key role in this identification process. Pattern analysis will certainly be necessary to accurately convey biometric data into real world, explainable stressors. 
   * Data Analysts
   * Program Flow:
      * Biometric data is collected from users via VR headset and stored in AWS backend
      * Analysts evaluate data to identify common stressors