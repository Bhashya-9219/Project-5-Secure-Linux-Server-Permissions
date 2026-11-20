# Project 5: Secure Linux Server Permissions

**Linux user and group management with file permissions and ACL-based access control.**

## 1. Objective
To implement user-based access restrictions on a Linux server and prevent unauthorized access to protected files and directories.

## 2. Tools Used
- Ubuntu Linux
- Linux Terminal
- User and Group Management
- chmod and chown
- Access Control Lists (ACL)

## 3. Implementation

- Created three Linux users:
  - `mbdevuser`
  - `mbtestuser`
  - `mbguestuser`
- Created two Linux groups:
  - `mbdevelopers`
  - `mbtesters`
- Assigned users to their respective groups.
- Created a protected directory at `/opt/project5`.
- Configured directory and file permissions using `chmod` and `chown`.
- Used ACL to provide read-only access to the tester group.

## 4. Access Control Configuration

| User | Read Access | Write Access |
|---|---|---|
| mbdevuser | Allowed | Allowed |
| mbtestuser | Allowed | Denied |
| mbguestuser | Denied | Denied |

## 5. Testing and Results

The following tests were performed:

- Developer successfully read the protected file and created a new file.
- Tester successfully read the protected file.
- Tester was denied permission when attempting to create a file.
- Guest user was denied access to the protected directory.

All access restrictions worked as expected.

## 6. Conclusion

Successfully implemented Linux user-based access restrictions using users, groups, standard file permissions and Access Control Lists (ACLs). This project demonstrated how Linux permissions help secure server resources and prevent unauthorized access.

## 7. Project Evidence

Screenshots are included in the `screenshots` folder to demonstrate:

1. User and group creation.
2. Directory and file permissions.
3. ACL configuration.
4. Successful and denied access tests.
