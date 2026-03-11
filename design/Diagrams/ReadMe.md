User Use Case
1. Register – Enables a new user to register in the MindCare system by providing requirement personal information.
2. Login – Enables a registered user to log in to the MindCare system securely using their account details.
3. Manage Account – Enables users to customize their account information, account privacy, and account security.
4. Chat with MindCare Assistant – Enables users to receive pre-programmed messages from MindCare assistants for support.
5. Record Mood – Enables users to input their emotional status for the day and possibly triggers for their emotional status in order to track their moods.
6. View Mood Insights – Displays a summary of a user’s moods for a week based on their previously recorded moods in order for them to be aware of their emotional status.
7.Connect with Therapist – This allows users to view the list of therapists based on their specialty, status, rating, and description, and request a counseling session with the therapist of their choice. 
8.Join Available Counseling Session – This allows users to book a counseling session with a therapist. This is specialized into Join Video Session and Join Text Session.
9.Perform Wind-Down Activities – This allows users to perform relaxing activities such as Do Breathing Exercise, Listen to Relaxing Music, Read Sleep Stories, and View Wind-Down Tips. 

Therapist Use Case
1.Manage Counselling Session Availability – This feature enables therapists to add available time slots for counselling sessions.
2.Conduct Counselling Sessions – Therapists can provide counselling support through Video Sessions and/or Text Sessions.

Payment System Use Case
1.Process Payment – This operation will enable the Payment System to securely process the user’s payment for the counselling session, verify the payment, and then send the confirmation back to the MindCare system to complete the booking process.

Use Case Diagram Explanation

The MindCare use case diagram shows how different actors interact with the system to promote mental health and wellness. In this case, two main actors are identified: the User and the Therapist, with one secondary actor: the Payment System.


In the use case diagram, the <<include>> arrow points from Login to Register, showing that the login process requires the user to register first if they do not already have an account. Conversely, for all other user actions — such as Manage Account, Chat with MindCare Assistant, Record Mood, View Mood Insights, Connect with Therapist, Join Available Counselling Session, and Perform Wind-Down Activities — the <<include>> arrows point from the action to Login, indicating that these features cannot be performed independently and require the user to be authenticated first. The <<include>> relationship in both cases represents a mandatory dependency, where the included use case must occur for the main use case to execute. 

Additionally, generalization is applied to the Join Available Counselling Session use case, which is specialized into Join Video Session and Join Text Session, and to the Perform Wind-Down Activities use case, which is specialized into different activity types such as Do Breathing Exercise, Listen to Relaxing Music, Read Sleep Stories, and View Wind-Down Tips. The main goals of joining counselling sessions and performing wellness activities can each be achieved through multiple methods, providing flexibility for user preferences while maintaining consistent functionality.


In the use case diagram, <<extend>> relationships are applied from Chat with MindCare Assistant, View Mood Insights, Connect with Therapist, and Perform Wind-Down Activities to the Record Mood use case. This indicates that recording a mood can optionally trigger these actions. For example, if a user records a “happy” mood, the system may display the View Mood Insights button, allowing the user to see a summary of their weekly emotional patterns. The <<extend>> relationship means that after a user records their mood, certain features may appear depending on the mood entered, offering helpful options to enhance the user’s experience.

The Therapist actor represents professional human support within the MindCare system. Therapists are responsible for managing counselling session availability and conducting counselling sessions with users. The Conduct Counselling Sessions use case is generalized into Video Sessions and Text Sessions, allowing flexibility based on user preferences. Video sessions provide more interactive communication, while text sessions offer a more private and convenient option. Although these therapist-related features were included in the system design, they were not implemented in the current prototype due to limited development time. They are planned to be implemented in the next sprint.
The Payment System acts as a secondary actor in the MindCare app, providing external support for processing payments. Its main use case, Process Payment, is included in the Join Counselling Session use case, indicating that completing a counselling session booking requires payment. This <<include>> relationship ensures that payment is a mandatory step for joining a counselling session, while allowing the system to integrate external transactional support effectively. The payment functionality is included in the system design but is not yet implemented in the current prototype and is planned for a future sprint.


In conclusion, the MindCare use case diagram illustrates a well-structured system where users, therapists, and the Payment System interact to support mental well-being, providing flexible features and accessible support for users.

