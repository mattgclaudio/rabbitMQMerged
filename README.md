# rabbitMQMerged
Code for database VM, only involved in authentication so dbServer just sets up a rabbitmq server listener and waits for an auth request through the rabbitvm server. should not process anything after that. Returns the two keys neccessary for accessing the alpaca trading API and performing actions through webVM/action.php. These are stored alongside the user's credentials in the database...which is probably not great security practice but i only have $20 in my actual account so hackers, go wild. 

IF IT RANDOMLY STOPS WORKING AND THE SERVICE WONT START, CHECK file ~/MYSQL/my.cnf, check the bind address
