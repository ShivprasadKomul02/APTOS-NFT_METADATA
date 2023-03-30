# APTOS-NFT_METADATA

Steps to follow:

1.Folllow above link to create resource account and mint nft to receiver
  https://aptos.dev/guides/move-guides/mint-nft-cli
  
 2.To run update metadata related function run below command
 
##For function with empty parameters
 aptos move run --function-id "resource-account-address"::create_nft_with_resource_account::"function_name" --profile nft-    receiver
  
  Ex:
  aptos move run --function-id "resource-account-address"::create_nft_with_resource_account::update_description --profile nft-receiver
  
 ##For parameterized function
  aptos move run --function-id "resource-account-address"::create_nft_with_resource_account::"function_name" --args "ParameterType":value --profile nft-receiver
  
  Ex:
  aptos move run --function-id "resource-account-address"::create_nft_with_resource_account::update_description --args String:"New description" --profile nft-receiver
  
  
