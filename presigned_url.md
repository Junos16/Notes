- It is important to have granular control over how or who can access objects in S3 buckets to prevent security issues in sensitive data. 3 ways access to objects in a bucket can be restricted:
    
    1. ***Permissions at the Bucket level***: 

        - To restrict/allow access to a large number of related objects at the same time, permissions for a whole bucket could be set by the owner.
        - When we have a lot of objects that we are accessing at the same time or accessing in the same way it is more convenient to set permissions at the bucket level
        - For example if we know in advance that we would always want to have a read only access to a large number of videos it is just more convenient to create an S3 bucket with read only access and store all of those videos there

    2. ***Permissions at the User level***: 

        - Another way to restrict/allow access to a large number of related objects at the same time is to set permissions for users that might have access to the bucket
        - When there are multiple consistent methods of access to a set of data we can set permissions at the user level instead of settings permissions for the whole bucket
        - For example if we have a video sharing service we might want to have two types of user level permissions: read only (for users who aren't original uploaders of the videos) and read and write (for users who have uploaded the videos) instead of setting permissions for the whole bucket containing all the videos

    3. ***Permissions at the object level***: 

        - The above two methods would prove to be very inflexible if we need a slight modification to how we access a small number of objects (or even a single object) in a bucket
        - We would either have to change the permissions of the entire bucket temporarily or create a new user just for this access
        - An alternative way to allow acces for this scenario is to set permissions at the object level as opposed to the bucket level or the user level
        - The owner could temporarily set permissions for a single object and allow users to access those objects with those sets of permissions irregardless of the permissions the user has or the whole bucket has
        - For example if the video sharing service has to censor a very sensitive video it might provide temporary read write access to a video to a moderator so that they can censor just the specific video without allowing them to have unrestricted access to censor other videos on the platform

- Presigned Urls: 
    - Presigned Urls are a way to provide permissions at the object level for objects in an S3 bucket
    - A user with the correct permissions to provide temporary object specific access can create such a url
    - The URL also includes other credentials to identify the object, the time for which people have access to the object and the specific HTTP methods that users would have access to for that object 
