# Kubectl commands
   ## Get all namespaces
    kubectl get namespace 
    
   ## Run/Get pods within a particular namespace
    kubectl run nginx --image=nginx --namespace=<insert-namespace-name>
    kubectl get pods --namespace=<insert-namespace-name>
    
   ## Permanently use a namespace
    kubectl config set-context --current --namespace=<insert-namespace-name-here>
    
   ## Validate a namespace
    kubectl config view --minify | grep namespace:
    
   ## Look for resources in/out of a namespace
    kubectl api-resources --namespaced=true
    kubectl api-resources --namespaced=false
    
   ## Get pods based on conditions
    kubectl get pods -l <set-based-conditions/equality-based-conditions>
    
   
   
    
   

