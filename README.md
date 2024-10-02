Group 46
Ananya Doshi, Riya Bihani, Vansh Dodiya

## Getting Started & Installation:

### Method 1:

This method requires:

```
    -Python 3.6 or greater
    -pip (or) pip3
```

1. Install the entire source code from this git repository as a zip file and extract it.
2. Install the necessary packages for the project using the following command -

```
pip install -r reqirements.txt
```

3. Setup the database using the following command -

```
python manage.py makemigrations
```

4. Create the superuser using the following command -

```
python manage.py createsuperuser
```

5. Finally start the server using the following command -

```
python manage.py runserver
```

6. Now the application is running on your local device and you can access the website by goign on the local host port:8000 of your device.

### Method 2:

1. Install the Docker Desktop application on your device.
2. Download the docker image file(.tar) using this link https://drive.google.com/file/d/1_-hrrcBlHTl3_KFKhyfN6XwS6KpcxVbP/view?usp=sharing
3. Build docker image using the following command -

```
docker build --tag <docker-image-name> .

# add the --network=host tag if you run into network problems
```

4. To execute the application, run the docker image which you just created using the following command -

```
docker run --publish 8000:8000 <docker-image-name>
```

5. Now the application is running inside the docker container and you can access the website by goign on the local host port:8000 of your device.

## Roadmap

### About WolfComplain3.0:

WolfComplain3.0 is an online platform used to organize and streamline doubt solving and class discussions for students at NC State University. It provides a centralized space where students can easily track all their questions and view doubts raised by their peers across various courses. By incorporating a tagging system, users can quickly identify the status of their inquiries and find relevant resources without the clutter often found in traditional learning management systems like Moodle. With WolfComplain3.0, students save valuable time by minimizing the need to navigate multiple platforms, allowing them to focus on their studies and enhance their learning experience. This platform fosters collaboration among students and faculty, ultimately creating a more productive and supportive educational environment.

### About WolfTrack 2.0:

1. Pagination of Search and Complaints
   Pagination is the process of displaying the data on multiple pages rather than showing them on a single page. Long pages take more time to load, and infinite pages need to load while the user scrolls, although this process isn't always flawless.

2. Filtering College Feed
   The college feed page now has filters to improve user experience and make it easier to search for a specific feed. There are three main filters on the application: department, type of feed, and college the feed is affiliated with.

3. Complaint Management and History
   Post complaints about certain topic and also view the previous complaints and their responses. Admin view for complaints and status view of all the complaints posted and the answers by the students.

4. Admin and Student Portal
   Admin and Student have different logins and the admins get graphs shown for the performance for past 6 months. Transferring a complain to principal if found unsolvable by teachers.

5. Personalized Dashboard
   Dashboard catered to the user and viewing the essential complaints and their responses. Viewing Solved, Rejected and Pending Complaints

### Future Scope

1. Email Notification on Complaint Resolution
   An email notification sent to the student who has raised a complaint stating that the complaint has been resolved and can be viewed by logging in to the system. Response of the complaint can also be viewed through the email recieved.

2. Bookmark Complaints of other Students
   Bookmarking or saving the complaints posted by other students for personal references and then viewing them whenever needed. Sorting and Searching in the saved complaints and filtering the complaint types in the bookmark section

3. Graphical Analysis of Complaint Response Time
   Provide a graph indicating the time taken by the professor to respond to the complaints. A six month graphical visualization for the professor to analyze the performance through the months.
