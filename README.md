# Oryx Build Timeout for Static Web Apps

If the below error is encountered when trying to build a Static web App. 

![image](https://user-images.githubusercontent.com/10644754/140665104-71c9a2f8-5d14-4f03-b414-da38691a504e.png)


The default Oryx build timeout of 15 minutes can be configured to suit the requirements. Valid values for the build timeout are 1 - 1440 minutes (although GitHub Actions may timeout before then). build_timeout_in_minutes can be added to the build and deploy step of the workflow.

```
 app_location: 'app' # App source code path
 api_location: 'api' # Api source code path - optional
 app_artifact_location: 'build' # Built app content directory - optional
 build_timeout_in_minutes: 15
 ```
