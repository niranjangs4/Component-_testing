Scanning

Advantages of Component testing
1.	Validate network level component test 
2.	Validate performance of build
3.	The early stage of build validation is the left shift (Component testing) is better than right shift (Integration testing)
4.	Left shift vs Right shift process:

    - In Right Shift: 
            -	Raise PR 
            -	Publish artifacts 
            -	Deployment to QA / Test Environment 
            -	Run integration testing found Bug
            -	Developer fix
            -	Create new artifacts and cycle repeats.
    
    -	In Left Shift: (Testing everything at PR Level):
              i.	Raise a PR
              ii.	Run component tests as a part of PR (Exhaustive set of test cases covering all the endpoints with all possible negative edge cases) 
              iii.	Found issue, PR is rejected. 
              iv.	Issues are fixed by dev and create a new PR. 
              v.	Artifact will only be released once component test / perf test passes. 
              vi.	This will reduce the release cycle time and help us find issues in the early life cycle of product development. 
      vii.	Less issues in QA / Test Environment.
    
Conclusion: instead of going through all process if right shift and finding issues we will validate initial PR level which saves a much time.
