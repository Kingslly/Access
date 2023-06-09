import json

def lambda_handler(event, context):

    
    body_part=json.loads(event['body'])
    
    repository_name=body_part['repository']['name']
    print("The repo name : {}".format(repository_name))
    
    count_of_stars=body_part['repository']['stargazers_count']
    print("The count of stars : {}".format(count_of_stars))
    
    user_who_gave_star=body_part['sender']['login']
    print("The user who gave star : {}".format(user_who_gave_star))
    
    url_of_the_user_who_gave_star=body_part['sender']['html_url']
    print("The profile of the user : {}".format(url_of_the_user_who_gave_star))
    
    return {
        'statusCode': 200,
        'body': json.dumps('Hello from Lambda!')
    }