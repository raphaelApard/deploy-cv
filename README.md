# Deploy CV

## Configuration serveur

    mkdir deploy.git
    cd deploy.git
    git init --bare

Créer le scrit sh : hooks/post-receive 
        
    chmod +x hooks/post-receive

## Configuration local
Ajout du remote git pour le déploiement

    git remote add production ssh://user@IP/root-path/git/nom-apprenant/deploy.git

## Utilisation

    git push production

## Ressources : 
    * https://www.digitalocean.com/community/tutorials/how-to-set-up-automatic-deployment-with-git-with-a-vps
    * https://coderwall.com/p/oj5smw/git-post-receive-hook-to-checkout-a-specific-branch
    * https://api.slack.com/incoming-webhooks
