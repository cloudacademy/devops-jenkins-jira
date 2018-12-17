//START-OF-SCRIPT
node {
    def JIRA_SITE_NAME = 'jira'
    def JIRA_PROJ_NAME = 'FIREAPP1'
    
    stage('JiraIssue'){
        def issue = [fields: [ project: [key: JIRA_PROJ_NAME],
                       summary: 'New JIRA Created from Jenkins.',
                       description: 'New JIRA Created from Jenkins.',
                       issuetype: [name: 'Task']]]
        
        def newIssue = jiraNewIssue issue: issue, site: JIRA_SITE_NAME
        
        echo newIssue.data.key
    }
}
//END-OF-SCRIPT