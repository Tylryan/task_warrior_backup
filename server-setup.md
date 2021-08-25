# Freecinc.com Server

If something goes wrong with your server, use a different one:
    - https://freecinc.com/generated_keys

# Don't copy this exactly. Use it a a guide 
1. Copy keys in ./task 
2. Set up Server settings
    Copy these commands line by line in your terminal
        - task config taskd.server freecinc.com:53589
        - task config taskd.key ~/.task/freecinc_3a250e28.key.pem
        - task config taskd.certificate ~/.task/freecinc_3a250e28.cert.pem
        - task config taskd.ca ~/.task/freecinc_3a250e28.ca.pem
        - task config taskd.credentials -- \
    'FreeCinc/freecinc_3a250e28/ba7c312a-0b3d-4659-a2f4-7085d0e015c9'

3. Make sure everything is working
- task diagnostics
    - CA, Cert, and Key should be readable
    - Server and Creds should have values

4. Sync your local files with the server
    - task sync init
