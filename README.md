# api documentation for  [vogels (v2.2.0)](https://github.com/ryanfitz/vogels#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-vogels.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-vogels) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vogels.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vogels)
#### DynamoDB data mapper

[![NPM](https://nodei.co/npm/vogels.png?downloads=true)](https://www.npmjs.com/package/vogels)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vogels/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-vogels_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vogels/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-vogels/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-vogels/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ryan Fitzgerald",
        "email": "ryan@codebrewstudios.com"
    },
    "bugs": {
        "url": "https://github.com/ryanfitz/vogels/issues"
    },
    "dependencies": {
        "async": "1.5.x",
        "aws-sdk": "2.2.x",
        "bunyan": "1.5.x",
        "joi": "5.x.x",
        "lodash": "3.10.x",
        "node-uuid": "1.4.x"
    },
    "description": "DynamoDB data mapper",
    "devDependencies": {
        "chai": "1.x.x",
        "istanbul": "^0.3.5",
        "jscoverage": "^0.5.9",
        "jshint": "2.x.x",
        "jshint-stylish": "2.x.x",
        "mocha": "2.x.x",
        "sinon": "1.12.x"
    },
    "directories": {},
    "dist": {
        "shasum": "ba02490c7ae5c9f51a41792b87d65d5911f793d4",
        "tarball": "https://registry.npmjs.org/vogels/-/vogels-2.2.0.tgz"
    },
    "engines": {
        "node": ">=0.10.30"
    },
    "gitHead": "e4ae788819244d35ccc7186dbe4b03937343294f",
    "homepage": "https://github.com/ryanfitz/vogels#readme",
    "keywords": [
        "datamapper",
        "DynamoDB",
        "aws",
        "amazon",
        "nosql"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "fitz",
            "email": "ryan@codebrewstudios.com"
        }
    ],
    "name": "vogels",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ryanfitz/vogels.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "2.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module vogels](#apidoc.module.vogels)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ACM ()](#apidoc.element.vogels.AWS.ACM)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.APIGateway ()](#apidoc.element.vogels.AWS.APIGateway)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.AutoScaling ()](#apidoc.element.vogels.AWS.AutoScaling)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFormation ()](#apidoc.element.vogels.AWS.CloudFormation)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFront ()](#apidoc.element.vogels.AWS.CloudFront)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudHSM ()](#apidoc.element.vogels.AWS.CloudHSM)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudSearch ()](#apidoc.element.vogels.AWS.CloudSearch)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudSearchDomain ()](#apidoc.element.vogels.AWS.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudTrail ()](#apidoc.element.vogels.AWS.CloudTrail)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatch ()](#apidoc.element.vogels.AWS.CloudWatch)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatchEvents ()](#apidoc.element.vogels.AWS.CloudWatchEvents)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatchLogs ()](#apidoc.element.vogels.AWS.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CodeCommit ()](#apidoc.element.vogels.AWS.CodeCommit)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CodeDeploy ()](#apidoc.element.vogels.AWS.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CodePipeline ()](#apidoc.element.vogels.AWS.CodePipeline)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoIdentity ()](#apidoc.element.vogels.AWS.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoIdentityCredentials (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoSync ()](#apidoc.element.vogels.AWS.CognitoSync)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Config (options)](#apidoc.element.vogels.AWS.Config)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ConfigService ()](#apidoc.element.vogels.AWS.ConfigService)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.CredentialProviderChain (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Credentials ()](#apidoc.element.vogels.AWS.Credentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DMS ()](#apidoc.element.vogels.AWS.DMS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DataPipeline ()](#apidoc.element.vogels.AWS.DataPipeline)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DeviceFarm ()](#apidoc.element.vogels.AWS.DeviceFarm)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DirectConnect ()](#apidoc.element.vogels.AWS.DirectConnect)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DirectoryService ()](#apidoc.element.vogels.AWS.DirectoryService)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDB ()](#apidoc.element.vogels.AWS.DynamoDB)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDBStreams ()](#apidoc.element.vogels.AWS.DynamoDBStreams)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.EC2 ()](#apidoc.element.vogels.AWS.EC2)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.EC2MetadataCredentials (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ECR ()](#apidoc.element.vogels.AWS.ECR)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ECS ()](#apidoc.element.vogels.AWS.ECS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.EFS ()](#apidoc.element.vogels.AWS.EFS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ELB ()](#apidoc.element.vogels.AWS.ELB)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.EMR ()](#apidoc.element.vogels.AWS.EMR)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ES ()](#apidoc.element.vogels.AWS.ES)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ElastiCache ()](#apidoc.element.vogels.AWS.ElastiCache)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ElasticBeanstalk ()](#apidoc.element.vogels.AWS.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ElasticTranscoder ()](#apidoc.element.vogels.AWS.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Endpoint (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.EnvironmentCredentials (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.FileSystemCredentials (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Firehose ()](#apidoc.element.vogels.AWS.Firehose)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.GameLift ()](#apidoc.element.vogels.AWS.GameLift)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Glacier ()](#apidoc.element.vogels.AWS.Glacier)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.HttpClient ()](#apidoc.element.vogels.AWS.HttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.HttpRequest (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.HttpResponse ()](#apidoc.element.vogels.AWS.HttpResponse)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.IAM ()](#apidoc.element.vogels.AWS.IAM)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ImportExport ()](#apidoc.element.vogels.AWS.ImportExport)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Inspector ()](#apidoc.element.vogels.AWS.Inspector)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Iot ()](#apidoc.element.vogels.AWS.Iot)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.IotData ()](#apidoc.element.vogels.AWS.IotData)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.KMS ()](#apidoc.element.vogels.AWS.KMS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Kinesis ()](#apidoc.element.vogels.AWS.Kinesis)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Lambda ()](#apidoc.element.vogels.AWS.Lambda)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.MachineLearning ()](#apidoc.element.vogels.AWS.MachineLearning)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.MarketplaceCommerceAnalytics ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.MarketplaceMetering ()](#apidoc.element.vogels.AWS.MarketplaceMetering)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.MetadataService (options)](#apidoc.element.vogels.AWS.MetadataService)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.MobileAnalytics ()](#apidoc.element.vogels.AWS.MobileAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.NodeHttpClient ()](#apidoc.element.vogels.AWS.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.OpsWorks ()](#apidoc.element.vogels.AWS.OpsWorks)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ParamValidator (validation)](#apidoc.element.vogels.AWS.ParamValidator)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.RDS ()](#apidoc.element.vogels.AWS.RDS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Redshift ()](#apidoc.element.vogels.AWS.Redshift)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Request (service, operation, params)](#apidoc.element.vogels.AWS.Request)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.ResourceWaiter (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Response (request)](#apidoc.element.vogels.AWS.Response)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Route53 ()](#apidoc.element.vogels.AWS.Route53)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Route53Domains ()](#apidoc.element.vogels.AWS.Route53Domains)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.S3 ()](#apidoc.element.vogels.AWS.S3)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SAMLCredentials (params)](#apidoc.element.vogels.AWS.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SES ()](#apidoc.element.vogels.AWS.SES)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SNS ()](#apidoc.element.vogels.AWS.SNS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SQS ()](#apidoc.element.vogels.AWS.SQS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SSM ()](#apidoc.element.vogels.AWS.SSM)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.STS ()](#apidoc.element.vogels.AWS.STS)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SWF ()](#apidoc.element.vogels.AWS.SWF)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SequentialExecutor ()](#apidoc.element.vogels.AWS.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Service (config)](#apidoc.element.vogels.AWS.Service)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SharedIniFileCredentials (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.SimpleDB ()](#apidoc.element.vogels.AWS.SimpleDB)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.StorageGateway ()](#apidoc.element.vogels.AWS.StorageGateway)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.Support ()](#apidoc.element.vogels.AWS.Support)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.TemporaryCredentials (params)](#apidoc.element.vogels.AWS.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.WAF ()](#apidoc.element.vogels.AWS.WAF)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.WebIdentityCredentials (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.</span>AWS.WorkSpaces ()](#apidoc.element.vogels.AWS.WorkSpaces)
1.  [function <span class="apidocSignatureSpan">vogels.</span>Set ()](#apidoc.element.vogels.Set)
1.  [function <span class="apidocSignatureSpan">vogels.</span>createTables (options, callback)](#apidoc.element.vogels.createTables)
1.  [function <span class="apidocSignatureSpan">vogels.</span>define (modelName, config)](#apidoc.element.vogels.define)
1.  [function <span class="apidocSignatureSpan">vogels.</span>documentClient (docClient)](#apidoc.element.vogels.documentClient)
1.  [function <span class="apidocSignatureSpan">vogels.</span>dynamoDriver (driver)](#apidoc.element.vogels.dynamoDriver)
1.  [function <span class="apidocSignatureSpan">vogels.</span>item (attrs, table)](#apidoc.element.vogels.item)
1.  [function <span class="apidocSignatureSpan">vogels.</span>model (name, model)](#apidoc.element.vogels.model)
1.  [function <span class="apidocSignatureSpan">vogels.</span>parallelScan (table, serializer, totalSegments)](#apidoc.element.vogels.parallelScan)
1.  [function <span class="apidocSignatureSpan">vogels.</span>query (hashKey, table, serializer)](#apidoc.element.vogels.query)
1.  [function <span class="apidocSignatureSpan">vogels.</span>reset ()](#apidoc.element.vogels.reset)
1.  [function <span class="apidocSignatureSpan">vogels.</span>scan (table, serializer)](#apidoc.element.vogels.scan)
1.  [function <span class="apidocSignatureSpan">vogels.</span>schema (config)](#apidoc.element.vogels.schema)
1.  [function <span class="apidocSignatureSpan">vogels.</span>table (name, schema, serializer, docClient, logger)](#apidoc.element.vogels.table)
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ACM.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.APIGateway.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.AutoScaling.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFormation.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFront.Signer.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFront.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudHSM.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudSearch.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudSearchDomain.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudTrail.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatch.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatchEvents.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatchLogs.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CodeCommit.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CodeDeploy.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CodePipeline.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoIdentity.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoIdentityCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoSync.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Config.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Config.prototype.keys
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ConfigService.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.CredentialProviderChain.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Credentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DMS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DataPipeline.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DeviceFarm.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DirectConnect.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DirectoryService.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDB.DocumentClient.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDB.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDBStreams.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.EC2.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.EC2MetadataCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ECR.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ECS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.EFS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ELB.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.EMR.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ES.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ElastiCache.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ElasticBeanstalk.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ElasticTranscoder.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Endpoint.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.EnvironmentCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.FileSystemCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Firehose.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.GameLift.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Glacier.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.HttpClient.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.HttpRequest.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.HttpResponse.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.IAM.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ImportExport.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Inspector.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Iot.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.IotData.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.JSON
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.JSON.Builder.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.JSON.Parser.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.KMS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Kinesis.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Lambda.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.MachineLearning.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.MarketplaceCommerceAnalytics.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.MarketplaceMetering.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.MetadataService.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.MobileAnalytics.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Model
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.OpsWorks.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ParamValidator.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.RDS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Redshift.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Request.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.ResourceWaiter.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Response.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Route53.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Route53Domains.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.S3.ManagedUpload.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.S3.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SAMLCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SES.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SNS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SQS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SSM.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.STS.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SWF.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SequentialExecutor.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Service.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SharedIniFileCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.Presign.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.RequestSigner.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.S3.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.V2.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.V3.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.V3Https.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Signers.V4.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.SimpleDB.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.StorageGateway.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.Support.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.TemporaryCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.WAF.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.WebIdentityCredentials.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.WorkSpaces.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.XML
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.XML.Builder.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.XML.Parser.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.util
1.  object <span class="apidocSignatureSpan">vogels.</span>AWS.util.Buffer.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>expressions
1.  object <span class="apidocSignatureSpan">vogels.</span>item.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>log
1.  object <span class="apidocSignatureSpan">vogels.</span>models
1.  object <span class="apidocSignatureSpan">vogels.</span>parallelScan.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>query.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>scan.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>schema.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>serializer
1.  object <span class="apidocSignatureSpan">vogels.</span>table.prototype
1.  object <span class="apidocSignatureSpan">vogels.</span>types
1.  object <span class="apidocSignatureSpan">vogels.</span>utils

#### [module vogels.AWS](#apidoc.module.vogels.AWS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ACM ()](#apidoc.element.vogels.AWS.ACM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>APIGateway ()](#apidoc.element.vogels.AWS.APIGateway)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>AutoScaling ()](#apidoc.element.vogels.AWS.AutoScaling)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFormation ()](#apidoc.element.vogels.AWS.CloudFormation)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFront ()](#apidoc.element.vogels.AWS.CloudFront)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudHSM ()](#apidoc.element.vogels.AWS.CloudHSM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearch ()](#apidoc.element.vogels.AWS.CloudSearch)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearchDomain ()](#apidoc.element.vogels.AWS.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudTrail ()](#apidoc.element.vogels.AWS.CloudTrail)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatch ()](#apidoc.element.vogels.AWS.CloudWatch)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchEvents ()](#apidoc.element.vogels.AWS.CloudWatchEvents)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchLogs ()](#apidoc.element.vogels.AWS.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeCommit ()](#apidoc.element.vogels.AWS.CodeCommit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeDeploy ()](#apidoc.element.vogels.AWS.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CodePipeline ()](#apidoc.element.vogels.AWS.CodePipeline)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentity ()](#apidoc.element.vogels.AWS.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoSync ()](#apidoc.element.vogels.AWS.CognitoSync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Config (options)](#apidoc.element.vogels.AWS.Config)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ConfigService ()](#apidoc.element.vogels.AWS.ConfigService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Credentials ()](#apidoc.element.vogels.AWS.Credentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DMS ()](#apidoc.element.vogels.AWS.DMS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DataPipeline ()](#apidoc.element.vogels.AWS.DataPipeline)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DeviceFarm ()](#apidoc.element.vogels.AWS.DeviceFarm)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectConnect ()](#apidoc.element.vogels.AWS.DirectConnect)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectoryService ()](#apidoc.element.vogels.AWS.DirectoryService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDB ()](#apidoc.element.vogels.AWS.DynamoDB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDBStreams ()](#apidoc.element.vogels.AWS.DynamoDBStreams)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2 ()](#apidoc.element.vogels.AWS.EC2)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ECR ()](#apidoc.element.vogels.AWS.ECR)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ECS ()](#apidoc.element.vogels.AWS.ECS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EFS ()](#apidoc.element.vogels.AWS.EFS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ELB ()](#apidoc.element.vogels.AWS.ELB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EMR ()](#apidoc.element.vogels.AWS.EMR)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ES ()](#apidoc.element.vogels.AWS.ES)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ElastiCache ()](#apidoc.element.vogels.AWS.ElastiCache)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticBeanstalk ()](#apidoc.element.vogels.AWS.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticTranscoder ()](#apidoc.element.vogels.AWS.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Firehose ()](#apidoc.element.vogels.AWS.Firehose)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>GameLift ()](#apidoc.element.vogels.AWS.GameLift)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Glacier ()](#apidoc.element.vogels.AWS.Glacier)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpClient ()](#apidoc.element.vogels.AWS.HttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpRequest (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpResponse ()](#apidoc.element.vogels.AWS.HttpResponse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>IAM ()](#apidoc.element.vogels.AWS.IAM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ImportExport ()](#apidoc.element.vogels.AWS.ImportExport)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Inspector ()](#apidoc.element.vogels.AWS.Inspector)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Iot ()](#apidoc.element.vogels.AWS.Iot)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>IotData ()](#apidoc.element.vogels.AWS.IotData)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>KMS ()](#apidoc.element.vogels.AWS.KMS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Kinesis ()](#apidoc.element.vogels.AWS.Kinesis)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Lambda ()](#apidoc.element.vogels.AWS.Lambda)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MachineLearning ()](#apidoc.element.vogels.AWS.MachineLearning)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceCommerceAnalytics ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceMetering ()](#apidoc.element.vogels.AWS.MarketplaceMetering)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MetadataService (options)](#apidoc.element.vogels.AWS.MetadataService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MobileAnalytics ()](#apidoc.element.vogels.AWS.MobileAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>NodeHttpClient ()](#apidoc.element.vogels.AWS.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>OpsWorks ()](#apidoc.element.vogels.AWS.OpsWorks)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ParamValidator (validation)](#apidoc.element.vogels.AWS.ParamValidator)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>RDS ()](#apidoc.element.vogels.AWS.RDS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Redshift ()](#apidoc.element.vogels.AWS.Redshift)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Request (service, operation, params)](#apidoc.element.vogels.AWS.Request)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Response (request)](#apidoc.element.vogels.AWS.Response)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53 ()](#apidoc.element.vogels.AWS.Route53)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53Domains ()](#apidoc.element.vogels.AWS.Route53Domains)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>S3 ()](#apidoc.element.vogels.AWS.S3)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SAMLCredentials (params)](#apidoc.element.vogels.AWS.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SES ()](#apidoc.element.vogels.AWS.SES)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SNS ()](#apidoc.element.vogels.AWS.SNS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SQS ()](#apidoc.element.vogels.AWS.SQS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SSM ()](#apidoc.element.vogels.AWS.SSM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>STS ()](#apidoc.element.vogels.AWS.STS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SWF ()](#apidoc.element.vogels.AWS.SWF)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SequentialExecutor ()](#apidoc.element.vogels.AWS.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Service (config)](#apidoc.element.vogels.AWS.Service)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SimpleDB ()](#apidoc.element.vogels.AWS.SimpleDB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>StorageGateway ()](#apidoc.element.vogels.AWS.StorageGateway)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Support ()](#apidoc.element.vogels.AWS.Support)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>TemporaryCredentials (params)](#apidoc.element.vogels.AWS.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>WAF ()](#apidoc.element.vogels.AWS.WAF)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>WorkSpaces ()](#apidoc.element.vogels.AWS.WorkSpaces)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>apiLoader (svc, version)](#apidoc.element.vogels.AWS.apiLoader)
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>EventListeners
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>JSON
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>Model
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>Protocol
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>Signers
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>XML
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>config
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>events
1.  object <span class="apidocSignatureSpan">vogels.AWS.</span>util
1.  string <span class="apidocSignatureSpan">vogels.AWS.</span>VERSION

#### [module vogels.AWS.ACM](#apidoc.module.vogels.AWS.ACM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ACM ()](#apidoc.element.vogels.AWS.ACM.ACM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ACM.</span>__super__ (config)](#apidoc.element.vogels.AWS.ACM.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ACM.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ACM.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ACM.</span>serviceIdentifier

#### [module vogels.AWS.ACM.prototype](#apidoc.module.vogels.AWS.ACM.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ACM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ACM.prototype.constructor)

#### [module vogels.AWS.APIGateway](#apidoc.module.vogels.AWS.APIGateway)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>APIGateway ()](#apidoc.element.vogels.AWS.APIGateway.APIGateway)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.</span>__super__ (config)](#apidoc.element.vogels.AWS.APIGateway.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.APIGateway.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.APIGateway.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.APIGateway.</span>serviceIdentifier

#### [module vogels.AWS.APIGateway.prototype](#apidoc.module.vogels.AWS.APIGateway.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.APIGateway.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.prototype.</span>setAcceptHeader (req)](#apidoc.element.vogels.AWS.APIGateway.prototype.setAcceptHeader)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.APIGateway.prototype.setupRequestListeners)

#### [module vogels.AWS.AutoScaling](#apidoc.module.vogels.AWS.AutoScaling)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>AutoScaling ()](#apidoc.element.vogels.AWS.AutoScaling.AutoScaling)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.</span>__super__ (config)](#apidoc.element.vogels.AWS.AutoScaling.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.</span>serviceIdentifier

#### [module vogels.AWS.AutoScaling.prototype](#apidoc.module.vogels.AWS.AutoScaling.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.AutoScaling.prototype.constructor)

#### [module vogels.AWS.CloudFormation](#apidoc.module.vogels.AWS.CloudFormation)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFormation ()](#apidoc.element.vogels.AWS.CloudFormation.CloudFormation)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudFormation.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.</span>serviceIdentifier

#### [module vogels.AWS.CloudFormation.prototype](#apidoc.module.vogels.AWS.CloudFormation.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudFormation.prototype.constructor)

#### [module vogels.AWS.CloudFront](#apidoc.module.vogels.AWS.CloudFront)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFront ()](#apidoc.element.vogels.AWS.CloudFront.CloudFront)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>Signer (keyPairId, privateKey)](#apidoc.element.vogels.AWS.CloudFront.Signer)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudFront.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>serviceIdentifier

#### [module vogels.AWS.CloudFront.Signer.prototype](#apidoc.module.vogels.AWS.CloudFront.Signer.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.Signer.prototype.</span>constructor (keyPairId, privateKey)](#apidoc.element.vogels.AWS.CloudFront.Signer.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.Signer.prototype.</span>getSignedCookie (options, cb)](#apidoc.element.vogels.AWS.CloudFront.Signer.prototype.getSignedCookie)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.Signer.prototype.</span>getSignedUrl (options, cb)](#apidoc.element.vogels.AWS.CloudFront.Signer.prototype.getSignedUrl)

#### [module vogels.AWS.CloudFront.prototype](#apidoc.module.vogels.AWS.CloudFront.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudFront.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.CloudFront.prototype.setupRequestListeners)

#### [module vogels.AWS.CloudHSM](#apidoc.module.vogels.AWS.CloudHSM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudHSM ()](#apidoc.element.vogels.AWS.CloudHSM.CloudHSM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudHSM.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.</span>serviceIdentifier

#### [module vogels.AWS.CloudHSM.prototype](#apidoc.module.vogels.AWS.CloudHSM.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudHSM.prototype.constructor)

#### [module vogels.AWS.CloudSearch](#apidoc.module.vogels.AWS.CloudSearch)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearch ()](#apidoc.element.vogels.AWS.CloudSearch.CloudSearch)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudSearch.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.</span>serviceIdentifier

#### [module vogels.AWS.CloudSearch.prototype](#apidoc.module.vogels.AWS.CloudSearch.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudSearch.prototype.constructor)

#### [module vogels.AWS.CloudSearchDomain](#apidoc.module.vogels.AWS.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearchDomain ()](#apidoc.element.vogels.AWS.CloudSearchDomain.CloudSearchDomain)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudSearchDomain.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.</span>serviceIdentifier

#### [module vogels.AWS.CloudSearchDomain.prototype](#apidoc.module.vogels.AWS.CloudSearchDomain.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>updateRegion (request)](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.updateRegion)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>validateCredentials (req, done)](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.validateCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.validateService)

#### [module vogels.AWS.CloudTrail](#apidoc.module.vogels.AWS.CloudTrail)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudTrail ()](#apidoc.element.vogels.AWS.CloudTrail.CloudTrail)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudTrail.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.</span>serviceIdentifier

#### [module vogels.AWS.CloudTrail.prototype](#apidoc.module.vogels.AWS.CloudTrail.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudTrail.prototype.constructor)

#### [module vogels.AWS.CloudWatch](#apidoc.module.vogels.AWS.CloudWatch)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatch ()](#apidoc.element.vogels.AWS.CloudWatch.CloudWatch)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudWatch.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.</span>serviceIdentifier

#### [module vogels.AWS.CloudWatch.prototype](#apidoc.module.vogels.AWS.CloudWatch.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudWatch.prototype.constructor)

#### [module vogels.AWS.CloudWatchEvents](#apidoc.module.vogels.AWS.CloudWatchEvents)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchEvents ()](#apidoc.element.vogels.AWS.CloudWatchEvents.CloudWatchEvents)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudWatchEvents.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.</span>serviceIdentifier

#### [module vogels.AWS.CloudWatchEvents.prototype](#apidoc.module.vogels.AWS.CloudWatchEvents.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudWatchEvents.prototype.constructor)

#### [module vogels.AWS.CloudWatchLogs](#apidoc.module.vogels.AWS.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchLogs ()](#apidoc.element.vogels.AWS.CloudWatchLogs.CloudWatchLogs)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudWatchLogs.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.</span>serviceIdentifier

#### [module vogels.AWS.CloudWatchLogs.prototype](#apidoc.module.vogels.AWS.CloudWatchLogs.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudWatchLogs.prototype.constructor)

#### [module vogels.AWS.CodeCommit](#apidoc.module.vogels.AWS.CodeCommit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeCommit ()](#apidoc.element.vogels.AWS.CodeCommit.CodeCommit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.</span>__super__ (config)](#apidoc.element.vogels.AWS.CodeCommit.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.</span>serviceIdentifier

#### [module vogels.AWS.CodeCommit.prototype](#apidoc.module.vogels.AWS.CodeCommit.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CodeCommit.prototype.constructor)

#### [module vogels.AWS.CodeDeploy](#apidoc.module.vogels.AWS.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeDeploy ()](#apidoc.element.vogels.AWS.CodeDeploy.CodeDeploy)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.</span>__super__ (config)](#apidoc.element.vogels.AWS.CodeDeploy.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.</span>serviceIdentifier

#### [module vogels.AWS.CodeDeploy.prototype](#apidoc.module.vogels.AWS.CodeDeploy.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CodeDeploy.prototype.constructor)

#### [module vogels.AWS.CodePipeline](#apidoc.module.vogels.AWS.CodePipeline)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CodePipeline ()](#apidoc.element.vogels.AWS.CodePipeline.CodePipeline)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.</span>__super__ (config)](#apidoc.element.vogels.AWS.CodePipeline.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.</span>serviceIdentifier

#### [module vogels.AWS.CodePipeline.prototype](#apidoc.module.vogels.AWS.CodePipeline.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CodePipeline.prototype.constructor)

#### [module vogels.AWS.CognitoIdentity](#apidoc.module.vogels.AWS.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentity ()](#apidoc.element.vogels.AWS.CognitoIdentity.CognitoIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.</span>__super__ (config)](#apidoc.element.vogels.AWS.CognitoIdentity.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.</span>serviceIdentifier

#### [module vogels.AWS.CognitoIdentity.prototype](#apidoc.module.vogels.AWS.CognitoIdentity.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>getCredentialsForIdentity (params, callback)](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.getCredentialsForIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>getId (params, callback)](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.getId)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>getOpenIdToken (params, callback)](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.getOpenIdToken)

#### [module vogels.AWS.CognitoIdentityCredentials](#apidoc.module.vogels.AWS.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.CognitoIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.__super__)

#### [module vogels.AWS.CognitoIdentityCredentials.prototype](#apidoc.module.vogels.AWS.CognitoIdentityCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>cacheId (data)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.cacheId)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>clearCachedId ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.clearCachedId)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.createClients)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getCredentialsForIdentity (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getCredentialsForIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getCredentialsFromSTS (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getCredentialsFromSTS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getId (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getId)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getStorage (key)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getStorage)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>loadCachedId ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.loadCachedId)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>loadCredentials (data, credentials)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.loadCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.refresh)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>setStorage (key, val)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.setStorage)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>localStorageKey
1.  object <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>storage

#### [module vogels.AWS.CognitoSync](#apidoc.module.vogels.AWS.CognitoSync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoSync ()](#apidoc.element.vogels.AWS.CognitoSync.CognitoSync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.</span>__super__ (config)](#apidoc.element.vogels.AWS.CognitoSync.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.</span>serviceIdentifier

#### [module vogels.AWS.CognitoSync.prototype](#apidoc.module.vogels.AWS.CognitoSync.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CognitoSync.prototype.constructor)

#### [module vogels.AWS.Config](#apidoc.module.vogels.AWS.Config)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Config (options)](#apidoc.element.vogels.AWS.Config.Config)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.</span>__super__ ()](#apidoc.element.vogels.AWS.Config.__super__)

#### [module vogels.AWS.Config.prototype](#apidoc.module.vogels.AWS.Config.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>clear ()](#apidoc.element.vogels.AWS.Config.prototype.clear)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.Config.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>extractCredentials (options)](#apidoc.element.vogels.AWS.Config.prototype.extractCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>getCredentials (callback)](#apidoc.element.vogels.AWS.Config.prototype.getCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>loadFromPath (path)](#apidoc.element.vogels.AWS.Config.prototype.loadFromPath)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>set (property, value, defaultValue)](#apidoc.element.vogels.AWS.Config.prototype.set)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>update (options, allowUnknownKeys)](#apidoc.element.vogels.AWS.Config.prototype.update)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>keys

#### [module vogels.AWS.Config.prototype.keys](#apidoc.module.vogels.AWS.Config.prototype.keys)
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>computeChecksums
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>convertResponseTypes
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>correctClockSkew
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>dynamoDbCrc32
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>paramValidation
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>s3BucketEndpoint
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>s3ForcePathStyle
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>signatureCache
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>sslEnabled
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>credentialProvider ()](#apidoc.element.vogels.AWS.Config.prototype.keys.credentialProvider)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>credentials ()](#apidoc.element.vogels.AWS.Config.prototype.keys.credentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>region ()](#apidoc.element.vogels.AWS.Config.prototype.keys.region)
1.  number <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>maxRedirects
1.  number <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>systemClockOffset
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>apiVersion
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>customUserAgent
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>httpOptions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>logger
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>retryDelayOptions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>signatureVersion

#### [module vogels.AWS.ConfigService](#apidoc.module.vogels.AWS.ConfigService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ConfigService ()](#apidoc.element.vogels.AWS.ConfigService.ConfigService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ConfigService.</span>__super__ (config)](#apidoc.element.vogels.AWS.ConfigService.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ConfigService.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ConfigService.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ConfigService.</span>serviceIdentifier

#### [module vogels.AWS.ConfigService.prototype](#apidoc.module.vogels.AWS.ConfigService.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ConfigService.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ConfigService.prototype.constructor)

#### [module vogels.AWS.CredentialProviderChain](#apidoc.module.vogels.AWS.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain.CredentialProviderChain)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.</span>__super__ ()](#apidoc.element.vogels.AWS.CredentialProviderChain.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.</span>defaultProviders

#### [module vogels.AWS.CredentialProviderChain.prototype](#apidoc.module.vogels.AWS.CredentialProviderChain.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.prototype.</span>constructor (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.prototype.</span>resolve (callback)](#apidoc.element.vogels.AWS.CredentialProviderChain.prototype.resolve)

#### [module vogels.AWS.Credentials](#apidoc.module.vogels.AWS.Credentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Credentials ()](#apidoc.element.vogels.AWS.Credentials.Credentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Credentials.</span>__super__ ()](#apidoc.element.vogels.AWS.Credentials.__super__)

#### [module vogels.AWS.Credentials.prototype](#apidoc.module.vogels.AWS.Credentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Credentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>get (callback)](#apidoc.element.vogels.AWS.Credentials.prototype.get)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>needsRefresh ()](#apidoc.element.vogels.AWS.Credentials.prototype.needsRefresh)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.Credentials.prototype.refresh)
1.  number <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>expiryWindow

#### [module vogels.AWS.DMS](#apidoc.module.vogels.AWS.DMS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DMS ()](#apidoc.element.vogels.AWS.DMS.DMS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DMS.</span>__super__ (config)](#apidoc.element.vogels.AWS.DMS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DMS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DMS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DMS.</span>serviceIdentifier

#### [module vogels.AWS.DMS.prototype](#apidoc.module.vogels.AWS.DMS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DMS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DMS.prototype.constructor)

#### [module vogels.AWS.DataPipeline](#apidoc.module.vogels.AWS.DataPipeline)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DataPipeline ()](#apidoc.element.vogels.AWS.DataPipeline.DataPipeline)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.</span>__super__ (config)](#apidoc.element.vogels.AWS.DataPipeline.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.</span>serviceIdentifier

#### [module vogels.AWS.DataPipeline.prototype](#apidoc.module.vogels.AWS.DataPipeline.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DataPipeline.prototype.constructor)

#### [module vogels.AWS.DeviceFarm](#apidoc.module.vogels.AWS.DeviceFarm)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DeviceFarm ()](#apidoc.element.vogels.AWS.DeviceFarm.DeviceFarm)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.</span>__super__ (config)](#apidoc.element.vogels.AWS.DeviceFarm.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.</span>serviceIdentifier

#### [module vogels.AWS.DeviceFarm.prototype](#apidoc.module.vogels.AWS.DeviceFarm.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DeviceFarm.prototype.constructor)

#### [module vogels.AWS.DirectConnect](#apidoc.module.vogels.AWS.DirectConnect)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectConnect ()](#apidoc.element.vogels.AWS.DirectConnect.DirectConnect)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.</span>__super__ (config)](#apidoc.element.vogels.AWS.DirectConnect.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.</span>serviceIdentifier

#### [module vogels.AWS.DirectConnect.prototype](#apidoc.module.vogels.AWS.DirectConnect.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DirectConnect.prototype.constructor)

#### [module vogels.AWS.DirectoryService](#apidoc.module.vogels.AWS.DirectoryService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectoryService ()](#apidoc.element.vogels.AWS.DirectoryService.DirectoryService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.</span>__super__ (config)](#apidoc.element.vogels.AWS.DirectoryService.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.</span>serviceIdentifier

#### [module vogels.AWS.DirectoryService.prototype](#apidoc.module.vogels.AWS.DirectoryService.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DirectoryService.prototype.constructor)

#### [module vogels.AWS.DynamoDB](#apidoc.module.vogels.AWS.DynamoDB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDB ()](#apidoc.element.vogels.AWS.DynamoDB.DynamoDB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>DocumentClient (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>__super__ (config)](#apidoc.element.vogels.AWS.DynamoDB.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>serviceIdentifier

#### [module vogels.AWS.DynamoDB.DocumentClient.prototype](#apidoc.module.vogels.AWS.DynamoDB.DocumentClient.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>batchGet (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.batchGet)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>batchWrite (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.batchWrite)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>bindServiceObject (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.bindServiceObject)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>configure (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.configure)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>createSet (list, options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.createSet)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>delete (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.delete)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>get (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.get)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>getTranslator ()](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.getTranslator)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>put (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.put)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>query (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.query)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>scan (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.scan)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>setupRequest (request)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.setupRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>setupResponse (request)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.setupResponse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>update (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.update)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>operations

#### [module vogels.AWS.DynamoDB.prototype](#apidoc.module.vogels.AWS.DynamoDB.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>checkCrc32 (resp)](#apidoc.element.vogels.AWS.DynamoDB.prototype.checkCrc32)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DynamoDB.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>crc32IsValid (resp)](#apidoc.element.vogels.AWS.DynamoDB.prototype.crc32IsValid)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>retryDelays (retryCount)](#apidoc.element.vogels.AWS.DynamoDB.prototype.retryDelays)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.DynamoDB.prototype.setupRequestListeners)
1.  number <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>defaultRetryCount

#### [module vogels.AWS.DynamoDBStreams](#apidoc.module.vogels.AWS.DynamoDBStreams)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDBStreams ()](#apidoc.element.vogels.AWS.DynamoDBStreams.DynamoDBStreams)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.</span>__super__ (config)](#apidoc.element.vogels.AWS.DynamoDBStreams.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.</span>serviceIdentifier

#### [module vogels.AWS.DynamoDBStreams.prototype](#apidoc.module.vogels.AWS.DynamoDBStreams.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DynamoDBStreams.prototype.constructor)

#### [module vogels.AWS.EC2](#apidoc.module.vogels.AWS.EC2)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2 ()](#apidoc.element.vogels.AWS.EC2.EC2)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2.</span>__super__ (config)](#apidoc.element.vogels.AWS.EC2.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.EC2.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.EC2.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.EC2.</span>serviceIdentifier

#### [module vogels.AWS.EC2.prototype](#apidoc.module.vogels.AWS.EC2.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>buildCopySnapshotPresignedUrl (req, done)](#apidoc.element.vogels.AWS.EC2.prototype.buildCopySnapshotPresignedUrl)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.EC2.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>extractError (resp)](#apidoc.element.vogels.AWS.EC2.prototype.extractError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.EC2.prototype.setupRequestListeners)

#### [module vogels.AWS.EC2MetadataCredentials](#apidoc.module.vogels.AWS.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials.EC2MetadataCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.EC2MetadataCredentials.__super__)

#### [module vogels.AWS.EC2MetadataCredentials.prototype](#apidoc.module.vogels.AWS.EC2MetadataCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.EC2MetadataCredentials.prototype.refresh)
1.  number <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.prototype.</span>defaultTimeout

#### [module vogels.AWS.ECR](#apidoc.module.vogels.AWS.ECR)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ECR ()](#apidoc.element.vogels.AWS.ECR.ECR)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ECR.</span>__super__ (config)](#apidoc.element.vogels.AWS.ECR.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ECR.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ECR.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ECR.</span>serviceIdentifier

#### [module vogels.AWS.ECR.prototype](#apidoc.module.vogels.AWS.ECR.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ECR.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ECR.prototype.constructor)

#### [module vogels.AWS.ECS](#apidoc.module.vogels.AWS.ECS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ECS ()](#apidoc.element.vogels.AWS.ECS.ECS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ECS.</span>__super__ (config)](#apidoc.element.vogels.AWS.ECS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ECS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ECS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ECS.</span>serviceIdentifier

#### [module vogels.AWS.ECS.prototype](#apidoc.module.vogels.AWS.ECS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ECS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ECS.prototype.constructor)

#### [module vogels.AWS.EFS](#apidoc.module.vogels.AWS.EFS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EFS ()](#apidoc.element.vogels.AWS.EFS.EFS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EFS.</span>__super__ (config)](#apidoc.element.vogels.AWS.EFS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.EFS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.EFS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.EFS.</span>serviceIdentifier

#### [module vogels.AWS.EFS.prototype](#apidoc.module.vogels.AWS.EFS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EFS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.EFS.prototype.constructor)

#### [module vogels.AWS.ELB](#apidoc.module.vogels.AWS.ELB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ELB ()](#apidoc.element.vogels.AWS.ELB.ELB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ELB.</span>__super__ (config)](#apidoc.element.vogels.AWS.ELB.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ELB.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ELB.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ELB.</span>serviceIdentifier

#### [module vogels.AWS.ELB.prototype](#apidoc.module.vogels.AWS.ELB.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ELB.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ELB.prototype.constructor)

#### [module vogels.AWS.EMR](#apidoc.module.vogels.AWS.EMR)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EMR ()](#apidoc.element.vogels.AWS.EMR.EMR)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EMR.</span>__super__ (config)](#apidoc.element.vogels.AWS.EMR.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.EMR.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.EMR.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.EMR.</span>serviceIdentifier

#### [module vogels.AWS.EMR.prototype](#apidoc.module.vogels.AWS.EMR.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EMR.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.EMR.prototype.constructor)

#### [module vogels.AWS.ES](#apidoc.module.vogels.AWS.ES)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ES ()](#apidoc.element.vogels.AWS.ES.ES)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ES.</span>__super__ (config)](#apidoc.element.vogels.AWS.ES.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ES.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ES.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ES.</span>serviceIdentifier

#### [module vogels.AWS.ES.prototype](#apidoc.module.vogels.AWS.ES.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ES.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ES.prototype.constructor)

#### [module vogels.AWS.ElastiCache](#apidoc.module.vogels.AWS.ElastiCache)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ElastiCache ()](#apidoc.element.vogels.AWS.ElastiCache.ElastiCache)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.</span>__super__ (config)](#apidoc.element.vogels.AWS.ElastiCache.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.</span>serviceIdentifier

#### [module vogels.AWS.ElastiCache.prototype](#apidoc.module.vogels.AWS.ElastiCache.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ElastiCache.prototype.constructor)

#### [module vogels.AWS.ElasticBeanstalk](#apidoc.module.vogels.AWS.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticBeanstalk ()](#apidoc.element.vogels.AWS.ElasticBeanstalk.ElasticBeanstalk)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.</span>__super__ (config)](#apidoc.element.vogels.AWS.ElasticBeanstalk.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.</span>serviceIdentifier

#### [module vogels.AWS.ElasticBeanstalk.prototype](#apidoc.module.vogels.AWS.ElasticBeanstalk.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ElasticBeanstalk.prototype.constructor)

#### [module vogels.AWS.ElasticTranscoder](#apidoc.module.vogels.AWS.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticTranscoder ()](#apidoc.element.vogels.AWS.ElasticTranscoder.ElasticTranscoder)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.</span>__super__ (config)](#apidoc.element.vogels.AWS.ElasticTranscoder.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.</span>serviceIdentifier

#### [module vogels.AWS.ElasticTranscoder.prototype](#apidoc.module.vogels.AWS.ElasticTranscoder.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ElasticTranscoder.prototype.constructor)

#### [module vogels.AWS.Endpoint](#apidoc.module.vogels.AWS.Endpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint.Endpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Endpoint.</span>__super__ ()](#apidoc.element.vogels.AWS.Endpoint.__super__)

#### [module vogels.AWS.Endpoint.prototype](#apidoc.module.vogels.AWS.Endpoint.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Endpoint.prototype.</span>constructor (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint.prototype.constructor)

#### [module vogels.AWS.EnvironmentCredentials](#apidoc.module.vogels.AWS.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials.EnvironmentCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EnvironmentCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.EnvironmentCredentials.__super__)

#### [module vogels.AWS.EnvironmentCredentials.prototype](#apidoc.module.vogels.AWS.EnvironmentCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EnvironmentCredentials.prototype.</span>constructor (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.EnvironmentCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.EnvironmentCredentials.prototype.refresh)

#### [module vogels.AWS.FileSystemCredentials](#apidoc.module.vogels.AWS.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials.FileSystemCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.FileSystemCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.FileSystemCredentials.__super__)

#### [module vogels.AWS.FileSystemCredentials.prototype](#apidoc.module.vogels.AWS.FileSystemCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.FileSystemCredentials.prototype.</span>constructor (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.FileSystemCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.FileSystemCredentials.prototype.refresh)

#### [module vogels.AWS.Firehose](#apidoc.module.vogels.AWS.Firehose)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Firehose ()](#apidoc.element.vogels.AWS.Firehose.Firehose)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Firehose.</span>__super__ (config)](#apidoc.element.vogels.AWS.Firehose.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Firehose.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Firehose.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Firehose.</span>serviceIdentifier

#### [module vogels.AWS.Firehose.prototype](#apidoc.module.vogels.AWS.Firehose.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Firehose.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Firehose.prototype.constructor)

#### [module vogels.AWS.GameLift](#apidoc.module.vogels.AWS.GameLift)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>GameLift ()](#apidoc.element.vogels.AWS.GameLift.GameLift)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.GameLift.</span>__super__ (config)](#apidoc.element.vogels.AWS.GameLift.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.GameLift.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.GameLift.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.GameLift.</span>serviceIdentifier

#### [module vogels.AWS.GameLift.prototype](#apidoc.module.vogels.AWS.GameLift.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.GameLift.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.GameLift.prototype.constructor)

#### [module vogels.AWS.Glacier](#apidoc.module.vogels.AWS.Glacier)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Glacier ()](#apidoc.element.vogels.AWS.Glacier.Glacier)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.</span>__super__ (config)](#apidoc.element.vogels.AWS.Glacier.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Glacier.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Glacier.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Glacier.</span>serviceIdentifier

#### [module vogels.AWS.Glacier.prototype](#apidoc.module.vogels.AWS.Glacier.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>addGlacierApiVersion (request)](#apidoc.element.vogels.AWS.Glacier.prototype.addGlacierApiVersion)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>addTreeHashHeaders (request)](#apidoc.element.vogels.AWS.Glacier.prototype.addTreeHashHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>buildHashTree (hashes)](#apidoc.element.vogels.AWS.Glacier.prototype.buildHashTree)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>computeChecksums (data)](#apidoc.element.vogels.AWS.Glacier.prototype.computeChecksums)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Glacier.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.Glacier.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>validateAccountId (request)](#apidoc.element.vogels.AWS.Glacier.prototype.validateAccountId)

#### [module vogels.AWS.HttpClient](#apidoc.module.vogels.AWS.HttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpClient ()](#apidoc.element.vogels.AWS.HttpClient.HttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.</span>__super__ ()](#apidoc.element.vogels.AWS.HttpClient.__super__)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.</span>getInstance ()](#apidoc.element.vogels.AWS.HttpClient.getInstance)
1.  number <span class="apidocSignatureSpan">vogels.AWS.HttpClient.</span>streamsApiVersion

#### [module vogels.AWS.HttpClient.prototype](#apidoc.module.vogels.AWS.HttpClient.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.HttpClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>handleRequest (httpRequest, httpOptions, callback, errCallback)](#apidoc.element.vogels.AWS.HttpClient.prototype.handleRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>progressStream (stream, httpRequest)](#apidoc.element.vogels.AWS.HttpClient.prototype.progressStream)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>sslAgent ()](#apidoc.element.vogels.AWS.HttpClient.prototype.sslAgent)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>writeBody (stream, httpRequest)](#apidoc.element.vogels.AWS.HttpClient.prototype.writeBody)
1.  object <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>emitter

#### [module vogels.AWS.HttpRequest](#apidoc.module.vogels.AWS.HttpRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpRequest (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest.HttpRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.</span>__super__ ()](#apidoc.element.vogels.AWS.HttpRequest.__super__)

#### [module vogels.AWS.HttpRequest.prototype](#apidoc.module.vogels.AWS.HttpRequest.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>constructor (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>pathname ()](#apidoc.element.vogels.AWS.HttpRequest.prototype.pathname)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>search ()](#apidoc.element.vogels.AWS.HttpRequest.prototype.search)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>setUserAgent (customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest.prototype.setUserAgent)

#### [module vogels.AWS.HttpResponse](#apidoc.module.vogels.AWS.HttpResponse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpResponse ()](#apidoc.element.vogels.AWS.HttpResponse.HttpResponse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpResponse.</span>__super__ ()](#apidoc.element.vogels.AWS.HttpResponse.__super__)

#### [module vogels.AWS.HttpResponse.prototype](#apidoc.module.vogels.AWS.HttpResponse.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpResponse.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.HttpResponse.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.HttpResponse.prototype.</span>createUnbufferedStream ()](#apidoc.element.vogels.AWS.HttpResponse.prototype.createUnbufferedStream)

#### [module vogels.AWS.IAM](#apidoc.module.vogels.AWS.IAM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>IAM ()](#apidoc.element.vogels.AWS.IAM.IAM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IAM.</span>__super__ (config)](#apidoc.element.vogels.AWS.IAM.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.IAM.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.IAM.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.IAM.</span>serviceIdentifier

#### [module vogels.AWS.IAM.prototype](#apidoc.module.vogels.AWS.IAM.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IAM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.IAM.prototype.constructor)

#### [module vogels.AWS.ImportExport](#apidoc.module.vogels.AWS.ImportExport)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ImportExport ()](#apidoc.element.vogels.AWS.ImportExport.ImportExport)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ImportExport.</span>__super__ (config)](#apidoc.element.vogels.AWS.ImportExport.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ImportExport.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.ImportExport.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.ImportExport.</span>serviceIdentifier

#### [module vogels.AWS.ImportExport.prototype](#apidoc.module.vogels.AWS.ImportExport.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ImportExport.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ImportExport.prototype.constructor)

#### [module vogels.AWS.Inspector](#apidoc.module.vogels.AWS.Inspector)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Inspector ()](#apidoc.element.vogels.AWS.Inspector.Inspector)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Inspector.</span>__super__ (config)](#apidoc.element.vogels.AWS.Inspector.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Inspector.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Inspector.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Inspector.</span>serviceIdentifier

#### [module vogels.AWS.Inspector.prototype](#apidoc.module.vogels.AWS.Inspector.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Inspector.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Inspector.prototype.constructor)

#### [module vogels.AWS.Iot](#apidoc.module.vogels.AWS.Iot)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Iot ()](#apidoc.element.vogels.AWS.Iot.Iot)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Iot.</span>__super__ (config)](#apidoc.element.vogels.AWS.Iot.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Iot.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Iot.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Iot.</span>serviceIdentifier

#### [module vogels.AWS.Iot.prototype](#apidoc.module.vogels.AWS.Iot.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Iot.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Iot.prototype.constructor)

#### [module vogels.AWS.IotData](#apidoc.module.vogels.AWS.IotData)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>IotData ()](#apidoc.element.vogels.AWS.IotData.IotData)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IotData.</span>__super__ (config)](#apidoc.element.vogels.AWS.IotData.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.IotData.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.IotData.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.IotData.</span>serviceIdentifier

#### [module vogels.AWS.IotData.prototype](#apidoc.module.vogels.AWS.IotData.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.IotData.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.IotData.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>validateResponseBody (resp)](#apidoc.element.vogels.AWS.IotData.prototype.validateResponseBody)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.IotData.prototype.validateService)

#### [module vogels.AWS.JSON](#apidoc.module.vogels.AWS.JSON)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.JSON.</span>Builder ()](#apidoc.element.vogels.AWS.JSON.Builder)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.JSON.</span>Parser ()](#apidoc.element.vogels.AWS.JSON.Parser)

#### [module vogels.AWS.JSON.Builder.prototype](#apidoc.module.vogels.AWS.JSON.Builder.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.JSON.Builder.prototype.</span>build (value, shape)](#apidoc.element.vogels.AWS.JSON.Builder.prototype.build)

#### [module vogels.AWS.JSON.Parser.prototype](#apidoc.module.vogels.AWS.JSON.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.JSON.Parser.prototype.</span>parse (value, shape)](#apidoc.element.vogels.AWS.JSON.Parser.prototype.parse)

#### [module vogels.AWS.KMS](#apidoc.module.vogels.AWS.KMS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>KMS ()](#apidoc.element.vogels.AWS.KMS.KMS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.KMS.</span>__super__ (config)](#apidoc.element.vogels.AWS.KMS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.KMS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.KMS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.KMS.</span>serviceIdentifier

#### [module vogels.AWS.KMS.prototype](#apidoc.module.vogels.AWS.KMS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.KMS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.KMS.prototype.constructor)

#### [module vogels.AWS.Kinesis](#apidoc.module.vogels.AWS.Kinesis)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Kinesis ()](#apidoc.element.vogels.AWS.Kinesis.Kinesis)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Kinesis.</span>__super__ (config)](#apidoc.element.vogels.AWS.Kinesis.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Kinesis.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Kinesis.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Kinesis.</span>serviceIdentifier

#### [module vogels.AWS.Kinesis.prototype](#apidoc.module.vogels.AWS.Kinesis.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Kinesis.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Kinesis.prototype.constructor)

#### [module vogels.AWS.Lambda](#apidoc.module.vogels.AWS.Lambda)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Lambda ()](#apidoc.element.vogels.AWS.Lambda.Lambda)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Lambda.</span>__super__ (config)](#apidoc.element.vogels.AWS.Lambda.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Lambda.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Lambda.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Lambda.</span>serviceIdentifier

#### [module vogels.AWS.Lambda.prototype](#apidoc.module.vogels.AWS.Lambda.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Lambda.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Lambda.prototype.constructor)

#### [module vogels.AWS.MachineLearning](#apidoc.module.vogels.AWS.MachineLearning)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MachineLearning ()](#apidoc.element.vogels.AWS.MachineLearning.MachineLearning)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.</span>__super__ (config)](#apidoc.element.vogels.AWS.MachineLearning.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.</span>serviceIdentifier

#### [module vogels.AWS.MachineLearning.prototype](#apidoc.module.vogels.AWS.MachineLearning.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.prototype.</span>buildEndpoint (request)](#apidoc.element.vogels.AWS.MachineLearning.prototype.buildEndpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MachineLearning.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.MachineLearning.prototype.setupRequestListeners)

#### [module vogels.AWS.MarketplaceCommerceAnalytics](#apidoc.module.vogels.AWS.MarketplaceCommerceAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceCommerceAnalytics ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.MarketplaceCommerceAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.</span>__super__ (config)](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.</span>serviceIdentifier

#### [module vogels.AWS.MarketplaceCommerceAnalytics.prototype](#apidoc.module.vogels.AWS.MarketplaceCommerceAnalytics.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.prototype.constructor)

#### [module vogels.AWS.MarketplaceMetering](#apidoc.module.vogels.AWS.MarketplaceMetering)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceMetering ()](#apidoc.element.vogels.AWS.MarketplaceMetering.MarketplaceMetering)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.</span>__super__ (config)](#apidoc.element.vogels.AWS.MarketplaceMetering.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.</span>serviceIdentifier

#### [module vogels.AWS.MarketplaceMetering.prototype](#apidoc.module.vogels.AWS.MarketplaceMetering.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MarketplaceMetering.prototype.constructor)

#### [module vogels.AWS.MetadataService](#apidoc.module.vogels.AWS.MetadataService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MetadataService (options)](#apidoc.element.vogels.AWS.MetadataService.MetadataService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.</span>__super__ ()](#apidoc.element.vogels.AWS.MetadataService.__super__)

#### [module vogels.AWS.MetadataService.prototype](#apidoc.module.vogels.AWS.MetadataService.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.MetadataService.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>loadCredentials (callback)](#apidoc.element.vogels.AWS.MetadataService.prototype.loadCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>request (path, callback)](#apidoc.element.vogels.AWS.MetadataService.prototype.request)
1.  object <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>httpOptions
1.  object <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>loadCredentialsCallbacks
1.  string <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>host

#### [module vogels.AWS.MobileAnalytics](#apidoc.module.vogels.AWS.MobileAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>MobileAnalytics ()](#apidoc.element.vogels.AWS.MobileAnalytics.MobileAnalytics)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.</span>__super__ (config)](#apidoc.element.vogels.AWS.MobileAnalytics.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.</span>serviceIdentifier

#### [module vogels.AWS.MobileAnalytics.prototype](#apidoc.module.vogels.AWS.MobileAnalytics.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MobileAnalytics.prototype.constructor)

#### [module vogels.AWS.Model](#apidoc.module.vogels.AWS.Model)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Api (api, options)](#apidoc.element.vogels.AWS.Model.Api)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Operation (name, operation, options)](#apidoc.element.vogels.AWS.Model.Operation)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Paginator (name, paginator)](#apidoc.element.vogels.AWS.Model.Paginator)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>ResourceWaiter (name, waiter, options)](#apidoc.element.vogels.AWS.Model.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Shape (shape, options, memberName)](#apidoc.element.vogels.AWS.Model.Shape)

#### [module vogels.AWS.NodeHttpClient](#apidoc.module.vogels.AWS.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>NodeHttpClient ()](#apidoc.element.vogels.AWS.NodeHttpClient.NodeHttpClient)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.NodeHttpClient.</span>__super__ ()](#apidoc.element.vogels.AWS.NodeHttpClient.__super__)

#### [module vogels.AWS.OpsWorks](#apidoc.module.vogels.AWS.OpsWorks)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>OpsWorks ()](#apidoc.element.vogels.AWS.OpsWorks.OpsWorks)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.</span>__super__ (config)](#apidoc.element.vogels.AWS.OpsWorks.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.</span>serviceIdentifier

#### [module vogels.AWS.OpsWorks.prototype](#apidoc.module.vogels.AWS.OpsWorks.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.OpsWorks.prototype.constructor)

#### [module vogels.AWS.ParamValidator](#apidoc.module.vogels.AWS.ParamValidator)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ParamValidator (validation)](#apidoc.element.vogels.AWS.ParamValidator.ParamValidator)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.</span>__super__ ()](#apidoc.element.vogels.AWS.ParamValidator.__super__)

#### [module vogels.AWS.ParamValidator.prototype](#apidoc.module.vogels.AWS.ParamValidator.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>constructor (validation)](#apidoc.element.vogels.AWS.ParamValidator.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>fail (code, message)](#apidoc.element.vogels.AWS.ParamValidator.prototype.fail)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validate (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validate)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateEnum (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateEnum)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateList (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateList)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateMap (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateMap)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateMember (shape, param, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateMember)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateNumber (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateNumber)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validatePattern (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validatePattern)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validatePayload (value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validatePayload)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateRange (shape, value, context, descriptor)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateRange)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateScalar (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateScalar)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateString (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateString)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateStructure (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateStructure)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateType (value, context, acceptedTypes, type)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateType)

#### [module vogels.AWS.RDS](#apidoc.module.vogels.AWS.RDS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>RDS ()](#apidoc.element.vogels.AWS.RDS.RDS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.RDS.</span>__super__ (config)](#apidoc.element.vogels.AWS.RDS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.RDS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.RDS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.RDS.</span>serviceIdentifier

#### [module vogels.AWS.RDS.prototype](#apidoc.module.vogels.AWS.RDS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.RDS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.RDS.prototype.constructor)

#### [module vogels.AWS.Redshift](#apidoc.module.vogels.AWS.Redshift)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Redshift ()](#apidoc.element.vogels.AWS.Redshift.Redshift)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Redshift.</span>__super__ (config)](#apidoc.element.vogels.AWS.Redshift.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Redshift.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Redshift.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Redshift.</span>serviceIdentifier

#### [module vogels.AWS.Redshift.prototype](#apidoc.module.vogels.AWS.Redshift.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Redshift.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Redshift.prototype.constructor)

#### [module vogels.AWS.Request](#apidoc.module.vogels.AWS.Request)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Request (service, operation, params)](#apidoc.element.vogels.AWS.Request.Request)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.</span>__super__ ()](#apidoc.element.vogels.AWS.Request.__super__)

#### [module vogels.AWS.Request.prototype](#apidoc.module.vogels.AWS.Request.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>abort ()](#apidoc.element.vogels.AWS.Request.prototype.abort)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addListener (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addListeners (listeners)](#apidoc.element.vogels.AWS.Request.prototype.addListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.vogels.AWS.Request.prototype.addNamedAsyncListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.vogels.AWS.Request.prototype.addNamedListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addNamedListeners (callback)](#apidoc.element.vogels.AWS.Request.prototype.addNamedListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>build (callback)](#apidoc.element.vogels.AWS.Request.prototype.build)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>buildAsGet (request)](#apidoc.element.vogels.AWS.Request.prototype.buildAsGet)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>callListeners (listeners, args, doneCallback, prevError)](#apidoc.element.vogels.AWS.Request.prototype.callListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>constructor (service, operation, params)](#apidoc.element.vogels.AWS.Request.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>createReadStream ()](#apidoc.element.vogels.AWS.Request.prototype.createReadStream)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>eachItem (callback)](#apidoc.element.vogels.AWS.Request.prototype.eachItem)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>eachPage (callback)](#apidoc.element.vogels.AWS.Request.prototype.eachPage)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.vogels.AWS.Request.prototype.emit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>emitEvent (eventName, args, done)](#apidoc.element.vogels.AWS.Request.prototype.emitEvent)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>eventParameters (eventName)](#apidoc.element.vogels.AWS.Request.prototype.eventParameters)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>haltHandlersOnError ()](#apidoc.element.vogels.AWS.Request.prototype.haltHandlersOnError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>isPageable ()](#apidoc.element.vogels.AWS.Request.prototype.isPageable)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>listeners (eventName)](#apidoc.element.vogels.AWS.Request.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>on (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.on)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>onAsync (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.onAsync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>presign (expires, callback)](#apidoc.element.vogels.AWS.Request.prototype.presign)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>removeAllListeners (eventName)](#apidoc.element.vogels.AWS.Request.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>removeListener (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>runTo (state, done)](#apidoc.element.vogels.AWS.Request.prototype.runTo)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>send (callback)](#apidoc.element.vogels.AWS.Request.prototype.send)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>toGet ()](#apidoc.element.vogels.AWS.Request.prototype.toGet)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>toUnauthenticated ()](#apidoc.element.vogels.AWS.Request.prototype.toUnauthenticated)

#### [module vogels.AWS.ResourceWaiter](#apidoc.module.vogels.AWS.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter.ResourceWaiter)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.</span>__super__ ()](#apidoc.element.vogels.AWS.ResourceWaiter.__super__)

#### [module vogels.AWS.ResourceWaiter.prototype](#apidoc.module.vogels.AWS.ResourceWaiter.prototype)
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>waitDone
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>checkError (resp)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.checkError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>checkSuccess (resp)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.checkSuccess)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>constructor (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>loadWaiterConfig (state, noException)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.loadWaiterConfig)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>setError (resp, retryable)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.setError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>wait (params, callback)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.wait)
1.  object <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>Listeners
1.  object <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>config
1.  object <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>expectedValue
1.  object <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>service
1.  object <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>state

#### [module vogels.AWS.Response](#apidoc.module.vogels.AWS.Response)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Response (request)](#apidoc.element.vogels.AWS.Response.Response)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Response.</span>__super__ ()](#apidoc.element.vogels.AWS.Response.__super__)

#### [module vogels.AWS.Response.prototype](#apidoc.module.vogels.AWS.Response.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>cacheNextPageTokens ()](#apidoc.element.vogels.AWS.Response.prototype.cacheNextPageTokens)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>constructor (request)](#apidoc.element.vogels.AWS.Response.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>hasNextPage ()](#apidoc.element.vogels.AWS.Response.prototype.hasNextPage)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>nextPage (callback)](#apidoc.element.vogels.AWS.Response.prototype.nextPage)

#### [module vogels.AWS.Route53](#apidoc.module.vogels.AWS.Route53)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53 ()](#apidoc.element.vogels.AWS.Route53.Route53)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Route53.</span>__super__ (config)](#apidoc.element.vogels.AWS.Route53.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Route53.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Route53.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Route53.</span>serviceIdentifier

#### [module vogels.AWS.Route53.prototype](#apidoc.module.vogels.AWS.Route53.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Route53.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Route53.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Route53.prototype.</span>sanitizeUrl (request)](#apidoc.element.vogels.AWS.Route53.prototype.sanitizeUrl)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Route53.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.Route53.prototype.setupRequestListeners)

#### [module vogels.AWS.Route53Domains](#apidoc.module.vogels.AWS.Route53Domains)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53Domains ()](#apidoc.element.vogels.AWS.Route53Domains.Route53Domains)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.</span>__super__ (config)](#apidoc.element.vogels.AWS.Route53Domains.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.</span>serviceIdentifier

#### [module vogels.AWS.Route53Domains.prototype](#apidoc.module.vogels.AWS.Route53Domains.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Route53Domains.prototype.constructor)

#### [module vogels.AWS.S3](#apidoc.module.vogels.AWS.S3)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>S3 ()](#apidoc.element.vogels.AWS.S3.S3)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.</span>ManagedUpload (options)](#apidoc.element.vogels.AWS.S3.ManagedUpload)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.</span>__super__ (config)](#apidoc.element.vogels.AWS.S3.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.S3.</span>serviceIdentifier

#### [module vogels.AWS.S3.ManagedUpload.prototype](#apidoc.module.vogels.AWS.S3.ManagedUpload.prototype)
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>failed
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>isDoneChunking
1.  boolean <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>leavePartsOnError
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>abort ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.abort)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addListener (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addListeners (listeners)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedAsyncListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addNamedListeners (callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>adjustTotalBytes ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.adjustTotalBytes)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>bindServiceObject (params)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.bindServiceObject)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>callListeners (listeners, args, doneCallback, prevError)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.callListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>cleanup (err)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.cleanup)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>configure (options)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.configure)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.emit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>fillBuffer ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.fillBuffer)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>fillStream ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.fillStream)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>finishMultiPart ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.finishMultiPart)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>finishSinglePart (err, data)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.finishSinglePart)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>listeners (eventName)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>nextChunk (chunk)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.nextChunk)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>on (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.on)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>onAsync (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.onAsync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>progress (info)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.progress)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>queueChunks (chunk, partNumber)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.queueChunks)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>removeAllListeners (eventName)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>removeListener (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>send (callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.send)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>uploadPart (chunk, partNumber)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.uploadPart)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>validateBody ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.validateBody)
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>activeParts
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>doneParts
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>maxTotalParts
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>minPartSize
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>numParts
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>partBufferLength
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>partPos
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>queueSize
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>totalChunkedBytes
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>totalPartNumbers
1.  number <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>totalUploadedBytes
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>completeInfo
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>multipartReq
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>partBuffers
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>partSize
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>parts

#### [module vogels.AWS.S3.prototype](#apidoc.module.vogels.AWS.S3.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>addContentType (req)](#apidoc.element.vogels.AWS.S3.prototype.addContentType)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>addExpect100Continue (req)](#apidoc.element.vogels.AWS.S3.prototype.addExpect100Continue)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>computeContentMd5 (req)](#apidoc.element.vogels.AWS.S3.prototype.computeContentMd5)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>computeSseCustomerKeyMd5 (req)](#apidoc.element.vogels.AWS.S3.prototype.computeSseCustomerKeyMd5)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.S3.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>createBucket (params, callback)](#apidoc.element.vogels.AWS.S3.prototype.createBucket)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>dnsCompatibleBucketName (bucketName)](#apidoc.element.vogels.AWS.S3.prototype.dnsCompatibleBucketName)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>extractData (resp)](#apidoc.element.vogels.AWS.S3.prototype.extractData)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>extractError (resp)](#apidoc.element.vogels.AWS.S3.prototype.extractError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>getSignedUrl (operation, params, callback)](#apidoc.element.vogels.AWS.S3.prototype.getSignedUrl)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>noPresignedContentLength (request)](#apidoc.element.vogels.AWS.S3.prototype.noPresignedContentLength)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>pathStyleBucketName (bucketName)](#apidoc.element.vogels.AWS.S3.prototype.pathStyleBucketName)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>populateURI (req)](#apidoc.element.vogels.AWS.S3.prototype.populateURI)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>prepareSignedUrl (request)](#apidoc.element.vogels.AWS.S3.prototype.prepareSignedUrl)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>retryableError (error, request)](#apidoc.element.vogels.AWS.S3.prototype.retryableError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.S3.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>successfulResponse (resp)](#apidoc.element.vogels.AWS.S3.prototype.successfulResponse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>upload (params, options, callback)](#apidoc.element.vogels.AWS.S3.prototype.upload)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>validateBucketEndpoint (req)](#apidoc.element.vogels.AWS.S3.prototype.validateBucketEndpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>validateScheme (req)](#apidoc.element.vogels.AWS.S3.prototype.validateScheme)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.S3.prototype.validateService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>willComputeChecksums (req)](#apidoc.element.vogels.AWS.S3.prototype.willComputeChecksums)
1.  object <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>computableChecksumOperations

#### [module vogels.AWS.SAMLCredentials](#apidoc.module.vogels.AWS.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SAMLCredentials (params)](#apidoc.element.vogels.AWS.SAMLCredentials.SAMLCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.SAMLCredentials.__super__)

#### [module vogels.AWS.SAMLCredentials.prototype](#apidoc.module.vogels.AWS.SAMLCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.SAMLCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.SAMLCredentials.prototype.createClients)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.SAMLCredentials.prototype.refresh)

#### [module vogels.AWS.SES](#apidoc.module.vogels.AWS.SES)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SES ()](#apidoc.element.vogels.AWS.SES.SES)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SES.</span>__super__ (config)](#apidoc.element.vogels.AWS.SES.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.SES.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.SES.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.SES.</span>serviceIdentifier

#### [module vogels.AWS.SES.prototype](#apidoc.module.vogels.AWS.SES.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SES.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SES.prototype.constructor)

#### [module vogels.AWS.SNS](#apidoc.module.vogels.AWS.SNS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SNS ()](#apidoc.element.vogels.AWS.SNS.SNS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SNS.</span>__super__ (config)](#apidoc.element.vogels.AWS.SNS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.SNS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.SNS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.SNS.</span>serviceIdentifier

#### [module vogels.AWS.SNS.prototype](#apidoc.module.vogels.AWS.SNS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SNS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SNS.prototype.constructor)

#### [module vogels.AWS.SQS](#apidoc.module.vogels.AWS.SQS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SQS ()](#apidoc.element.vogels.AWS.SQS.SQS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.</span>__super__ (config)](#apidoc.element.vogels.AWS.SQS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.SQS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.SQS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.SQS.</span>serviceIdentifier

#### [module vogels.AWS.SQS.prototype](#apidoc.module.vogels.AWS.SQS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>buildEndpoint (request)](#apidoc.element.vogels.AWS.SQS.prototype.buildEndpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>calculateChecksum (data)](#apidoc.element.vogels.AWS.SQS.prototype.calculateChecksum)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SQS.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>isChecksumValid (checksum, data)](#apidoc.element.vogels.AWS.SQS.prototype.isChecksumValid)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.SQS.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>throwInvalidChecksumError (response, ids, message)](#apidoc.element.vogels.AWS.SQS.prototype.throwInvalidChecksumError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>verifyReceiveMessageChecksum (response)](#apidoc.element.vogels.AWS.SQS.prototype.verifyReceiveMessageChecksum)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>verifySendMessageBatchChecksum (response)](#apidoc.element.vogels.AWS.SQS.prototype.verifySendMessageBatchChecksum)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>verifySendMessageChecksum (response)](#apidoc.element.vogels.AWS.SQS.prototype.verifySendMessageChecksum)

#### [module vogels.AWS.SSM](#apidoc.module.vogels.AWS.SSM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SSM ()](#apidoc.element.vogels.AWS.SSM.SSM)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SSM.</span>__super__ (config)](#apidoc.element.vogels.AWS.SSM.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.SSM.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.SSM.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.SSM.</span>serviceIdentifier

#### [module vogels.AWS.SSM.prototype](#apidoc.module.vogels.AWS.SSM.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SSM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SSM.prototype.constructor)

#### [module vogels.AWS.STS](#apidoc.module.vogels.AWS.STS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>STS ()](#apidoc.element.vogels.AWS.STS.STS)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.STS.</span>__super__ (config)](#apidoc.element.vogels.AWS.STS.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.STS.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.STS.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.STS.</span>serviceIdentifier

#### [module vogels.AWS.STS.prototype](#apidoc.module.vogels.AWS.STS.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>assumeRoleWithSAML (params, callback)](#apidoc.element.vogels.AWS.STS.prototype.assumeRoleWithSAML)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>assumeRoleWithWebIdentity (params, callback)](#apidoc.element.vogels.AWS.STS.prototype.assumeRoleWithWebIdentity)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.STS.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>credentialsFrom (data, credentials)](#apidoc.element.vogels.AWS.STS.prototype.credentialsFrom)

#### [module vogels.AWS.SWF](#apidoc.module.vogels.AWS.SWF)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SWF ()](#apidoc.element.vogels.AWS.SWF.SWF)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SWF.</span>__super__ (config)](#apidoc.element.vogels.AWS.SWF.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.SWF.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.SWF.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.SWF.</span>serviceIdentifier

#### [module vogels.AWS.SWF.prototype](#apidoc.module.vogels.AWS.SWF.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SWF.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SWF.prototype.constructor)

#### [module vogels.AWS.SequentialExecutor](#apidoc.module.vogels.AWS.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SequentialExecutor ()](#apidoc.element.vogels.AWS.SequentialExecutor.SequentialExecutor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.</span>__super__ ()](#apidoc.element.vogels.AWS.SequentialExecutor.__super__)

#### [module vogels.AWS.SequentialExecutor.prototype](#apidoc.module.vogels.AWS.SequentialExecutor.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addListener (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addListeners (listeners)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedAsyncListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedListener)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addNamedListeners (callback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>callListeners (listeners, args, doneCallback, prevError)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.callListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.emit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>listeners (eventName)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>on (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.on)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>onAsync (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.onAsync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>removeAllListeners (eventName)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>removeListener (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.removeListener)

#### [module vogels.AWS.Service](#apidoc.module.vogels.AWS.Service)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Service (config)](#apidoc.element.vogels.AWS.Service.Service)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>__super__ ()](#apidoc.element.vogels.AWS.Service.__super__)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>addVersions (svc, versions)](#apidoc.element.vogels.AWS.Service.addVersions)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>defineMethods (svc)](#apidoc.element.vogels.AWS.Service.defineMethods)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>defineService (serviceIdentifier, versions, features)](#apidoc.element.vogels.AWS.Service.defineService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>defineServiceApi (superclass, version, apiConfig)](#apidoc.element.vogels.AWS.Service.defineServiceApi)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>hasService (identifier)](#apidoc.element.vogels.AWS.Service.hasService)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Service.</span>_serviceMap

#### [module vogels.AWS.Service.prototype](#apidoc.module.vogels.AWS.Service.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>addAllRequestListeners (request)](#apidoc.element.vogels.AWS.Service.prototype.addAllRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>clockSkewError (error)](#apidoc.element.vogels.AWS.Service.prototype.clockSkewError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>constructor (config)](#apidoc.element.vogels.AWS.Service.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>endpointFromTemplate (endpoint)](#apidoc.element.vogels.AWS.Service.prototype.endpointFromTemplate)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>expiredCredentialsError (error)](#apidoc.element.vogels.AWS.Service.prototype.expiredCredentialsError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>getLatestServiceClass (version)](#apidoc.element.vogels.AWS.Service.prototype.getLatestServiceClass)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>getLatestServiceVersion (version)](#apidoc.element.vogels.AWS.Service.prototype.getLatestServiceVersion)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>getSignerClass ()](#apidoc.element.vogels.AWS.Service.prototype.getSignerClass)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>initialize (config)](#apidoc.element.vogels.AWS.Service.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>loadServiceClass (serviceConfig)](#apidoc.element.vogels.AWS.Service.prototype.loadServiceClass)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>makeRequest (operation, params, callback)](#apidoc.element.vogels.AWS.Service.prototype.makeRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>makeUnauthenticatedRequest (operation, params, callback)](#apidoc.element.vogels.AWS.Service.prototype.makeUnauthenticatedRequest)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>networkingError (error)](#apidoc.element.vogels.AWS.Service.prototype.networkingError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>numRetries ()](#apidoc.element.vogels.AWS.Service.prototype.numRetries)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>paginationConfig (operation, throwException)](#apidoc.element.vogels.AWS.Service.prototype.paginationConfig)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>retryDelays (retryCount)](#apidoc.element.vogels.AWS.Service.prototype.retryDelays)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>retryableError (error)](#apidoc.element.vogels.AWS.Service.prototype.retryableError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>serviceInterface ()](#apidoc.element.vogels.AWS.Service.prototype.serviceInterface)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>setEndpoint (endpoint)](#apidoc.element.vogels.AWS.Service.prototype.setEndpoint)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>setupRequestListeners ()](#apidoc.element.vogels.AWS.Service.prototype.setupRequestListeners)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>successfulResponse (resp)](#apidoc.element.vogels.AWS.Service.prototype.successfulResponse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>throttledError (error)](#apidoc.element.vogels.AWS.Service.prototype.throttledError)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.Service.prototype.validateService)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>waitFor (state, params, callback)](#apidoc.element.vogels.AWS.Service.prototype.waitFor)
1.  number <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>defaultRetryCount
1.  object <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>api

#### [module vogels.AWS.SharedIniFileCredentials](#apidoc.module.vogels.AWS.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials.SharedIniFileCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.SharedIniFileCredentials.__super__)

#### [module vogels.AWS.SharedIniFileCredentials.prototype](#apidoc.module.vogels.AWS.SharedIniFileCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.prototype.</span>loadDefaultFilename ()](#apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.loadDefaultFilename)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.refresh)

#### [module vogels.AWS.Signers](#apidoc.module.vogels.AWS.Signers)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>Presign ()](#apidoc.element.vogels.AWS.Signers.Presign)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>RequestSigner (request)](#apidoc.element.vogels.AWS.Signers.RequestSigner)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>S3 ()](#apidoc.element.vogels.AWS.Signers.S3)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V2 ()](#apidoc.element.vogels.AWS.Signers.V2)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V3 ()](#apidoc.element.vogels.AWS.Signers.V3)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V3Https ()](#apidoc.element.vogels.AWS.Signers.V3Https)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V4 (request, serviceName, signatureCache)](#apidoc.element.vogels.AWS.Signers.V4)

#### [module vogels.AWS.Signers.Presign.prototype](#apidoc.module.vogels.AWS.Signers.Presign.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.Presign.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.Presign.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.Presign.prototype.</span>sign (request, expireTime, callback)](#apidoc.element.vogels.AWS.Signers.Presign.prototype.sign)

#### [module vogels.AWS.Signers.RequestSigner.prototype](#apidoc.module.vogels.AWS.Signers.RequestSigner.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.RequestSigner.prototype.</span>constructor (request)](#apidoc.element.vogels.AWS.Signers.RequestSigner.prototype.constructor)

#### [module vogels.AWS.Signers.S3.prototype](#apidoc.module.vogels.AWS.Signers.S3.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.S3.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>canonicalizedAmzHeaders ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.canonicalizedAmzHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>canonicalizedResource ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.canonicalizedResource)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>sign (secret, string)](#apidoc.element.vogels.AWS.Signers.S3.prototype.sign)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.stringToSign)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>responseHeaders
1.  object <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>subResources

#### [module vogels.AWS.Signers.V2.prototype](#apidoc.module.vogels.AWS.Signers.V2.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.V2.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.V2.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>signature (credentials)](#apidoc.element.vogels.AWS.Signers.V2.prototype.signature)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.V2.prototype.stringToSign)

#### [module vogels.AWS.Signers.V3.prototype](#apidoc.module.vogels.AWS.Signers.V3.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.V3.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>authorization (credentials)](#apidoc.element.vogels.AWS.Signers.V3.prototype.authorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>canonicalHeaders ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.canonicalHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>headersToSign ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.headersToSign)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>signature (credentials)](#apidoc.element.vogels.AWS.Signers.V3.prototype.signature)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>signedHeaders ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.signedHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.stringToSign)

#### [module vogels.AWS.Signers.V3Https.prototype](#apidoc.module.vogels.AWS.Signers.V3Https.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3Https.prototype.</span>authorization (credentials)](#apidoc.element.vogels.AWS.Signers.V3Https.prototype.authorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3Https.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.V3Https.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3Https.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.V3Https.prototype.stringToSign)

#### [module vogels.AWS.Signers.V4.prototype](#apidoc.module.vogels.AWS.Signers.V4.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.V4.prototype.addAuthorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>addHeaders (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.addHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>authorization (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.authorization)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>canonicalHeaderValues (values)](#apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalHeaderValues)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>canonicalHeaders ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>canonicalString ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalString)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>constructor (request, serviceName, signatureCache)](#apidoc.element.vogels.AWS.Signers.V4.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>credentialString (datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.credentialString)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>hexEncodedBodyHash ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.hexEncodedBodyHash)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>hexEncodedHash (string)](#apidoc.element.vogels.AWS.Signers.V4.prototype.hexEncodedHash)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>isPresigned ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.isPresigned)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>isSignableHeader (key)](#apidoc.element.vogels.AWS.Signers.V4.prototype.isSignableHeader)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>signature (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.signature)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>signedHeaders ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.signedHeaders)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>stringToSign (datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.stringToSign)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>updateForPresigned (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.updateForPresigned)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>unsignableHeaders
1.  string <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>algorithm

#### [module vogels.AWS.SimpleDB](#apidoc.module.vogels.AWS.SimpleDB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>SimpleDB ()](#apidoc.element.vogels.AWS.SimpleDB.SimpleDB)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.</span>__super__ (config)](#apidoc.element.vogels.AWS.SimpleDB.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.</span>serviceIdentifier

#### [module vogels.AWS.SimpleDB.prototype](#apidoc.module.vogels.AWS.SimpleDB.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SimpleDB.prototype.constructor)

#### [module vogels.AWS.StorageGateway](#apidoc.module.vogels.AWS.StorageGateway)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>StorageGateway ()](#apidoc.element.vogels.AWS.StorageGateway.StorageGateway)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.</span>__super__ (config)](#apidoc.element.vogels.AWS.StorageGateway.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.</span>serviceIdentifier

#### [module vogels.AWS.StorageGateway.prototype](#apidoc.module.vogels.AWS.StorageGateway.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.StorageGateway.prototype.constructor)

#### [module vogels.AWS.Support](#apidoc.module.vogels.AWS.Support)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>Support ()](#apidoc.element.vogels.AWS.Support.Support)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Support.</span>__super__ (config)](#apidoc.element.vogels.AWS.Support.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.Support.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.Support.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.Support.</span>serviceIdentifier

#### [module vogels.AWS.Support.prototype](#apidoc.module.vogels.AWS.Support.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.Support.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Support.prototype.constructor)

#### [module vogels.AWS.TemporaryCredentials](#apidoc.module.vogels.AWS.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>TemporaryCredentials (params)](#apidoc.element.vogels.AWS.TemporaryCredentials.TemporaryCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.TemporaryCredentials.__super__)

#### [module vogels.AWS.TemporaryCredentials.prototype](#apidoc.module.vogels.AWS.TemporaryCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.createClients)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>loadMasterCredentials ()](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.loadMasterCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.refresh)

#### [module vogels.AWS.WAF](#apidoc.module.vogels.AWS.WAF)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>WAF ()](#apidoc.element.vogels.AWS.WAF.WAF)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WAF.</span>__super__ (config)](#apidoc.element.vogels.AWS.WAF.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.WAF.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.WAF.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.WAF.</span>serviceIdentifier

#### [module vogels.AWS.WAF.prototype](#apidoc.module.vogels.AWS.WAF.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WAF.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.WAF.prototype.constructor)

#### [module vogels.AWS.WebIdentityCredentials](#apidoc.module.vogels.AWS.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials.WebIdentityCredentials)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.WebIdentityCredentials.__super__)

#### [module vogels.AWS.WebIdentityCredentials.prototype](#apidoc.module.vogels.AWS.WebIdentityCredentials.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.createClients)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.refresh)

#### [module vogels.AWS.WorkSpaces](#apidoc.module.vogels.AWS.WorkSpaces)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.</span>WorkSpaces ()](#apidoc.element.vogels.AWS.WorkSpaces.WorkSpaces)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.</span>__super__ (config)](#apidoc.element.vogels.AWS.WorkSpaces.__super__)
1.  object <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.</span>apiVersions
1.  object <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.</span>services
1.  string <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.</span>serviceIdentifier

#### [module vogels.AWS.WorkSpaces.prototype](#apidoc.module.vogels.AWS.WorkSpaces.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.WorkSpaces.prototype.constructor)

#### [module vogels.AWS.XML](#apidoc.module.vogels.AWS.XML)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.XML.</span>Builder ()](#apidoc.element.vogels.AWS.XML.Builder)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.XML.</span>Parser ()](#apidoc.element.vogels.AWS.XML.Parser)

#### [module vogels.AWS.XML.Builder.prototype](#apidoc.module.vogels.AWS.XML.Builder.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.XML.Builder.prototype.</span>toXML (params, shape, rootElement, noEmpty)](#apidoc.element.vogels.AWS.XML.Builder.prototype.toXML)

#### [module vogels.AWS.XML.Parser.prototype](#apidoc.module.vogels.AWS.XML.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.XML.Parser.prototype.</span>parse (xml, shape)](#apidoc.element.vogels.AWS.XML.Parser.prototype.parse)

#### [module vogels.AWS.util](#apidoc.module.vogels.AWS.util)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.vogels.AWS.util.Buffer)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>applyClockOffset (serverTime)](#apidoc.element.vogels.AWS.util.applyClockOffset)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>arrayEach (array, iterFunction)](#apidoc.element.vogels.AWS.util.arrayEach)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>arraySliceFn (obj)](#apidoc.element.vogels.AWS.util.arraySliceFn)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>computeSha256 (body, done)](#apidoc.element.vogels.AWS.util.computeSha256)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>copy (object)](#apidoc.element.vogels.AWS.util.copy)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>each (object, iterFunction)](#apidoc.element.vogels.AWS.util.each)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>engine ()](#apidoc.element.vogels.AWS.util.engine)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>error (err, options)](#apidoc.element.vogels.AWS.util.error)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>extractRequestId (resp)](#apidoc.element.vogels.AWS.util.extractRequestId)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>hideProperties (obj, props)](#apidoc.element.vogels.AWS.util.hideProperties)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>hoistPayloadMember (resp)](#apidoc.element.vogels.AWS.util.hoistPayloadMember)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>inherit (klass, features)](#apidoc.element.vogels.AWS.util.inherit)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isBrowser ()](#apidoc.element.vogels.AWS.util.isBrowser)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isClockSkewed (serverTime)](#apidoc.element.vogels.AWS.util.isClockSkewed)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isEmpty (obj)](#apidoc.element.vogels.AWS.util.isEmpty)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isNode ()](#apidoc.element.vogels.AWS.util.isNode)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isType (obj, type)](#apidoc.element.vogels.AWS.util.isType)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>memoizedProperty (obj, name, get, enumerable)](#apidoc.element.vogels.AWS.util.memoizedProperty)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>merge (obj1, obj2)](#apidoc.element.vogels.AWS.util.merge)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>mixin ()](#apidoc.element.vogels.AWS.util.mixin)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>multiRequire (module1, module2)](#apidoc.element.vogels.AWS.util.multiRequire)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>nodeRequire (module)](#apidoc.element.vogels.AWS.util.nodeRequire)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>property (obj, name, value, enumerable, isValue)](#apidoc.element.vogels.AWS.util.property)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>queryParamsToString (params)](#apidoc.element.vogels.AWS.util.queryParamsToString)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>queryStringParse (qs)](#apidoc.element.vogels.AWS.util.queryStringParse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>readFileSync (path)](#apidoc.element.vogels.AWS.util.readFileSync)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>typeName (type)](#apidoc.element.vogels.AWS.util.typeName)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>update (obj1, obj2)](#apidoc.element.vogels.AWS.util.update)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>uriEscape (string)](#apidoc.element.vogels.AWS.util.uriEscape)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>uriEscapePath (string)](#apidoc.element.vogels.AWS.util.uriEscapePath)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>urlFormat (url)](#apidoc.element.vogels.AWS.util.urlFormat)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>urlParse (url)](#apidoc.element.vogels.AWS.util.urlParse)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.</span>userAgent ()](#apidoc.element.vogels.AWS.util.userAgent)
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>abort
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>base64
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>buffer
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>crypto
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>date
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>fn
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>ini
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>jamespath
1.  object <span class="apidocSignatureSpan">vogels.AWS.util.</span>string

#### [module vogels.AWS.util.Buffer.prototype](#apidoc.module.vogels.AWS.util.Buffer.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.asciiSlice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.asciiWrite)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>base64Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.base64Slice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>base64Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.base64Write)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.vogels.AWS.util.Buffer.prototype.compare)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>copy ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.copy)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>equals (b)](#apidoc.element.vogels.AWS.util.Buffer.prototype.equals)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.fill)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>hexSlice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.hexSlice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>hexWrite ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.hexWrite)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.includes)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>inspect ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.latin1Slice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>latin1Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.latin1Write)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readDoubleBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readDoubleLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readFloatBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readFloatLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt16BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt16LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt32BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt32LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt8)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readIntBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readIntLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt16BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt16LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt32BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt32LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt8)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUIntBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUIntLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>slice (start, end)](#apidoc.element.vogels.AWS.util.Buffer.prototype.slice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>swap16 ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.swap16)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>swap32 ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.swap32)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>swap64 ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.swap64)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>toJSON ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>toString ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.ucs2Slice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.ucs2Write)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.utf8Slice)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>utf8Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.utf8Write)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.write)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeDoubleBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeDoubleLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeFloatBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeFloatLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt16BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt16LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt32BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt32LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt8)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeIntBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeIntLE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt16BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt16LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt32BE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt32LE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt8)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUIntBE)
1.  [function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUIntLE)

#### [module vogels.expressions](#apidoc.module.vogels.expressions)
1.  [function <span class="apidocSignatureSpan">vogels.expressions.</span>buildFilterExpression (key, operator, existingValueNames, val1, val2 )](#apidoc.element.vogels.expressions.buildFilterExpression)
1.  [function <span class="apidocSignatureSpan">vogels.expressions.</span>parse (str)](#apidoc.element.vogels.expressions.parse)
1.  [function <span class="apidocSignatureSpan">vogels.expressions.</span>serializeUpdateExpression (schema, item)](#apidoc.element.vogels.expressions.serializeUpdateExpression)
1.  [function <span class="apidocSignatureSpan">vogels.expressions.</span>stringify (expressions)](#apidoc.element.vogels.expressions.stringify)

#### [module vogels.item](#apidoc.module.vogels.item)
1.  [function <span class="apidocSignatureSpan">vogels.</span>item (attrs, table)](#apidoc.element.vogels.item.item)
1.  [function <span class="apidocSignatureSpan">vogels.item.</span>super_ ()](#apidoc.element.vogels.item.super_)

#### [module vogels.item.prototype](#apidoc.module.vogels.item.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.item.prototype.</span>destroy (options, callback)](#apidoc.element.vogels.item.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">vogels.item.prototype.</span>get (key)](#apidoc.element.vogels.item.prototype.get)
1.  [function <span class="apidocSignatureSpan">vogels.item.prototype.</span>save (callback)](#apidoc.element.vogels.item.prototype.save)
1.  [function <span class="apidocSignatureSpan">vogels.item.prototype.</span>set (params)](#apidoc.element.vogels.item.prototype.set)
1.  [function <span class="apidocSignatureSpan">vogels.item.prototype.</span>toJSON ()](#apidoc.element.vogels.item.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">vogels.item.prototype.</span>update (options, callback)](#apidoc.element.vogels.item.prototype.update)

#### [module vogels.parallelScan](#apidoc.module.vogels.parallelScan)
1.  [function <span class="apidocSignatureSpan">vogels.</span>parallelScan (table, serializer, totalSegments)](#apidoc.element.vogels.parallelScan.parallelScan)
1.  [function <span class="apidocSignatureSpan">vogels.parallelScan.</span>super_ (table, serializer)](#apidoc.element.vogels.parallelScan.super_)

#### [module vogels.parallelScan.prototype](#apidoc.module.vogels.parallelScan.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.parallelScan.prototype.</span>exec (callback)](#apidoc.element.vogels.parallelScan.prototype.exec)

#### [module vogels.query](#apidoc.module.vogels.query)
1.  [function <span class="apidocSignatureSpan">vogels.</span>query (hashKey, table, serializer)](#apidoc.element.vogels.query.query)

#### [module vogels.query.prototype](#apidoc.module.vogels.query.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>addFilterCondition (condition)](#apidoc.element.vogels.query.prototype.addFilterCondition)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>addKeyCondition (condition)](#apidoc.element.vogels.query.prototype.addKeyCondition)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>ascending ()](#apidoc.element.vogels.query.prototype.ascending)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>attributes (attrs)](#apidoc.element.vogels.query.prototype.attributes)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>buildKey ()](#apidoc.element.vogels.query.prototype.buildKey)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>buildRequest ()](#apidoc.element.vogels.query.prototype.buildRequest)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>consistentRead (read)](#apidoc.element.vogels.query.prototype.consistentRead)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>descending ()](#apidoc.element.vogels.query.prototype.descending)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>exec (callback)](#apidoc.element.vogels.query.prototype.exec)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>expressionAttributeNames (data)](#apidoc.element.vogels.query.prototype.expressionAttributeNames)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>expressionAttributeValues (data)](#apidoc.element.vogels.query.prototype.expressionAttributeValues)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>filter (keyName)](#apidoc.element.vogels.query.prototype.filter)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>filterExpression (expression)](#apidoc.element.vogels.query.prototype.filterExpression)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>limit (num)](#apidoc.element.vogels.query.prototype.limit)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>loadAll ()](#apidoc.element.vogels.query.prototype.loadAll)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>projectionExpression (data)](#apidoc.element.vogels.query.prototype.projectionExpression)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>returnConsumedCapacity (value)](#apidoc.element.vogels.query.prototype.returnConsumedCapacity)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>select (value)](#apidoc.element.vogels.query.prototype.select)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>startKey (hashKey, rangeKey)](#apidoc.element.vogels.query.prototype.startKey)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>usingIndex (name)](#apidoc.element.vogels.query.prototype.usingIndex)
1.  [function <span class="apidocSignatureSpan">vogels.query.prototype.</span>where (keyName)](#apidoc.element.vogels.query.prototype.where)

#### [module vogels.scan](#apidoc.module.vogels.scan)
1.  [function <span class="apidocSignatureSpan">vogels.</span>scan (table, serializer)](#apidoc.element.vogels.scan.scan)

#### [module vogels.scan.prototype](#apidoc.module.vogels.scan.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>addFilterCondition (condition)](#apidoc.element.vogels.scan.prototype.addFilterCondition)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>attributes (attrs)](#apidoc.element.vogels.scan.prototype.attributes)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>buildRequest ()](#apidoc.element.vogels.scan.prototype.buildRequest)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>exec (callback)](#apidoc.element.vogels.scan.prototype.exec)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>expressionAttributeNames (data)](#apidoc.element.vogels.scan.prototype.expressionAttributeNames)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>expressionAttributeValues (data)](#apidoc.element.vogels.scan.prototype.expressionAttributeValues)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>filterExpression (expression)](#apidoc.element.vogels.scan.prototype.filterExpression)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>limit (num)](#apidoc.element.vogels.scan.prototype.limit)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>loadAll ()](#apidoc.element.vogels.scan.prototype.loadAll)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>projectionExpression (data)](#apidoc.element.vogels.scan.prototype.projectionExpression)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>returnConsumedCapacity (value)](#apidoc.element.vogels.scan.prototype.returnConsumedCapacity)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>segments (segment, totalSegments)](#apidoc.element.vogels.scan.prototype.segments)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>select (value)](#apidoc.element.vogels.scan.prototype.select)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>startKey (hashKey, rangeKey)](#apidoc.element.vogels.scan.prototype.startKey)
1.  [function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>where (keyName)](#apidoc.element.vogels.scan.prototype.where)

#### [module vogels.schema](#apidoc.module.vogels.schema)
1.  [function <span class="apidocSignatureSpan">vogels.</span>schema (config)](#apidoc.element.vogels.schema.schema)
1.  object <span class="apidocSignatureSpan">vogels.schema.</span>types

#### [module vogels.schema.prototype](#apidoc.module.vogels.schema.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.schema.prototype.</span>applyDefaults (data)](#apidoc.element.vogels.schema.prototype.applyDefaults)
1.  [function <span class="apidocSignatureSpan">vogels.schema.prototype.</span>validate (params, options)](#apidoc.element.vogels.schema.prototype.validate)

#### [module vogels.serializer](#apidoc.module.vogels.serializer)
1.  [function <span class="apidocSignatureSpan">vogels.serializer.</span>buildKey (hashKey, rangeKey, schema)](#apidoc.element.vogels.serializer.buildKey)
1.  [function <span class="apidocSignatureSpan">vogels.serializer.</span>deserializeItem (item)](#apidoc.element.vogels.serializer.deserializeItem)
1.  [function <span class="apidocSignatureSpan">vogels.serializer.</span>serializeAttribute (value, type, options)](#apidoc.element.vogels.serializer.serializeAttribute)
1.  [function <span class="apidocSignatureSpan">vogels.serializer.</span>serializeItem (schema, item, options)](#apidoc.element.vogels.serializer.serializeItem)
1.  [function <span class="apidocSignatureSpan">vogels.serializer.</span>serializeItemForUpdate (schema, action, item)](#apidoc.element.vogels.serializer.serializeItemForUpdate)

#### [module vogels.table](#apidoc.module.vogels.table)
1.  [function <span class="apidocSignatureSpan">vogels.</span>table (name, schema, serializer, docClient, logger)](#apidoc.element.vogels.table.table)

#### [module vogels.table.prototype](#apidoc.module.vogels.table.prototype)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>create (item, options, callback)](#apidoc.element.vogels.table.prototype.create)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>createTable (options, callback)](#apidoc.element.vogels.table.prototype.createTable)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>deleteTable (callback)](#apidoc.element.vogels.table.prototype.deleteTable)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>describeTable (callback)](#apidoc.element.vogels.table.prototype.describeTable)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>destroy (hashKey, rangeKey, options, callback)](#apidoc.element.vogels.table.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>get (hashKey, rangeKey, options, callback)](#apidoc.element.vogels.table.prototype.get)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>initItem (attrs)](#apidoc.element.vogels.table.prototype.initItem)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>parallelScan (totalSegments)](#apidoc.element.vogels.table.prototype.parallelScan)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>query (hashKey)](#apidoc.element.vogels.table.prototype.query)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>runBatchGetItems (params, callback)](#apidoc.element.vogels.table.prototype.runBatchGetItems)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>runQuery (params, callback)](#apidoc.element.vogels.table.prototype.runQuery)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>runScan (params, callback)](#apidoc.element.vogels.table.prototype.runScan)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>scan ()](#apidoc.element.vogels.table.prototype.scan)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>sendRequest (method, params, callback)](#apidoc.element.vogels.table.prototype.sendRequest)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>tableName ()](#apidoc.element.vogels.table.prototype.tableName)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>update (item, options, callback)](#apidoc.element.vogels.table.prototype.update)
1.  [function <span class="apidocSignatureSpan">vogels.table.prototype.</span>updateTable (throughput, callback)](#apidoc.element.vogels.table.prototype.updateTable)

#### [module vogels.types](#apidoc.module.vogels.types)
1.  [function <span class="apidocSignatureSpan">vogels.types.</span>binarySet ()](#apidoc.element.vogels.types.binarySet)
1.  [function <span class="apidocSignatureSpan">vogels.types.</span>numberSet ()](#apidoc.element.vogels.types.numberSet)
1.  [function <span class="apidocSignatureSpan">vogels.types.</span>stringSet ()](#apidoc.element.vogels.types.stringSet)
1.  [function <span class="apidocSignatureSpan">vogels.types.</span>timeUUID ()](#apidoc.element.vogels.types.timeUUID)
1.  [function <span class="apidocSignatureSpan">vogels.types.</span>uuid ()](#apidoc.element.vogels.types.uuid)

#### [module vogels.utils](#apidoc.module.vogels.utils)
1.  [function <span class="apidocSignatureSpan">vogels.utils.</span>mergeResults (responses, tableName)](#apidoc.element.vogels.utils.mergeResults)
1.  [function <span class="apidocSignatureSpan">vogels.utils.</span>omitNulls (data)](#apidoc.element.vogels.utils.omitNulls)
1.  [function <span class="apidocSignatureSpan">vogels.utils.</span>omitPrimaryKeys (schema, params)](#apidoc.element.vogels.utils.omitPrimaryKeys)
1.  [function <span class="apidocSignatureSpan">vogels.utils.</span>paginatedRequest (self, runRequestFunc, callback)](#apidoc.element.vogels.utils.paginatedRequest)
1.  [function <span class="apidocSignatureSpan">vogels.utils.</span>strToBin (value)](#apidoc.element.vogels.utils.strToBin)
1.  [function <span class="apidocSignatureSpan">vogels.utils.</span>streamRequest (self, runRequestFunc)](#apidoc.element.vogels.utils.streamRequest)



# <a name="apidoc.module.vogels"></a>[module vogels](#apidoc.module.vogels)

#### <a name="apidoc.element.vogels.AWS.ACM"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ACM ()](#apidoc.element.vogels.AWS.ACM)
- description and source-code
```javascript
AWS.ACM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.APIGateway"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.APIGateway ()](#apidoc.element.vogels.AWS.APIGateway)
- description and source-code
```javascript
AWS.APIGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.AutoScaling"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.AutoScaling ()](#apidoc.element.vogels.AWS.AutoScaling)
- description and source-code
```javascript
AWS.AutoScaling = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFormation"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFormation ()](#apidoc.element.vogels.AWS.CloudFormation)
- description and source-code
```javascript
AWS.CloudFormation = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudFront ()](#apidoc.element.vogels.AWS.CloudFront)
- description and source-code
```javascript
AWS.CloudFront = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudHSM"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudHSM ()](#apidoc.element.vogels.AWS.CloudHSM)
- description and source-code
```javascript
AWS.CloudHSM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearch"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudSearch ()](#apidoc.element.vogels.AWS.CloudSearch)
- description and source-code
```javascript
AWS.CloudSearch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudSearchDomain ()](#apidoc.element.vogels.AWS.CloudSearchDomain)
- description and source-code
```javascript
AWS.CloudSearchDomain = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudTrail"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudTrail ()](#apidoc.element.vogels.AWS.CloudTrail)
- description and source-code
```javascript
AWS.CloudTrail = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatch"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatch ()](#apidoc.element.vogels.AWS.CloudWatch)
- description and source-code
```javascript
AWS.CloudWatch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatchEvents"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatchEvents ()](#apidoc.element.vogels.AWS.CloudWatchEvents)
- description and source-code
```javascript
AWS.CloudWatchEvents = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatchLogs"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CloudWatchLogs ()](#apidoc.element.vogels.AWS.CloudWatchLogs)
- description and source-code
```javascript
AWS.CloudWatchLogs = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodeCommit"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CodeCommit ()](#apidoc.element.vogels.AWS.CodeCommit)
- description and source-code
```javascript
AWS.CodeCommit = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodeDeploy"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CodeDeploy ()](#apidoc.element.vogels.AWS.CodeDeploy)
- description and source-code
```javascript
AWS.CodeDeploy = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodePipeline"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CodePipeline ()](#apidoc.element.vogels.AWS.CodePipeline)
- description and source-code
```javascript
AWS.CodePipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoIdentity ()](#apidoc.element.vogels.AWS.CognitoIdentity)
- description and source-code
```javascript
AWS.CognitoIdentity = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoIdentityCredentials (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoSync"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CognitoSync ()](#apidoc.element.vogels.AWS.CognitoSync)
- description and source-code
```javascript
AWS.CognitoSync = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Config (options)](#apidoc.element.vogels.AWS.Config)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ConfigService"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ConfigService ()](#apidoc.element.vogels.AWS.ConfigService)
- description and source-code
```javascript
AWS.ConfigService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CredentialProviderChain"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.CredentialProviderChain (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Credentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Credentials ()](#apidoc.element.vogels.AWS.Credentials)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DMS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DMS ()](#apidoc.element.vogels.AWS.DMS)
- description and source-code
```javascript
AWS.DMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DataPipeline"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DataPipeline ()](#apidoc.element.vogels.AWS.DataPipeline)
- description and source-code
```javascript
AWS.DataPipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DeviceFarm"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DeviceFarm ()](#apidoc.element.vogels.AWS.DeviceFarm)
- description and source-code
```javascript
AWS.DeviceFarm = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DirectConnect"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DirectConnect ()](#apidoc.element.vogels.AWS.DirectConnect)
- description and source-code
```javascript
AWS.DirectConnect = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DirectoryService"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DirectoryService ()](#apidoc.element.vogels.AWS.DirectoryService)
- description and source-code
```javascript
AWS.DirectoryService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDB ()](#apidoc.element.vogels.AWS.DynamoDB)
- description and source-code
```javascript
AWS.DynamoDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDBStreams"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.DynamoDBStreams ()](#apidoc.element.vogels.AWS.DynamoDBStreams)
- description and source-code
```javascript
AWS.DynamoDBStreams = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.EC2 ()](#apidoc.element.vogels.AWS.EC2)
- description and source-code
```javascript
AWS.EC2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2MetadataCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.EC2MetadataCredentials (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ECR"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ECR ()](#apidoc.element.vogels.AWS.ECR)
- description and source-code
```javascript
AWS.ECR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ECS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ECS ()](#apidoc.element.vogels.AWS.ECS)
- description and source-code
```javascript
AWS.ECS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EFS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.EFS ()](#apidoc.element.vogels.AWS.EFS)
- description and source-code
```javascript
AWS.EFS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ELB"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ELB ()](#apidoc.element.vogels.AWS.ELB)
- description and source-code
```javascript
AWS.ELB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EMR"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.EMR ()](#apidoc.element.vogels.AWS.EMR)
- description and source-code
```javascript
AWS.EMR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ES"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ES ()](#apidoc.element.vogels.AWS.ES)
- description and source-code
```javascript
AWS.ES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElastiCache"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ElastiCache ()](#apidoc.element.vogels.AWS.ElastiCache)
- description and source-code
```javascript
AWS.ElastiCache = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElasticBeanstalk"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ElasticBeanstalk ()](#apidoc.element.vogels.AWS.ElasticBeanstalk)
- description and source-code
```javascript
AWS.ElasticBeanstalk = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElasticTranscoder"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ElasticTranscoder ()](#apidoc.element.vogels.AWS.ElasticTranscoder)
- description and source-code
```javascript
AWS.ElasticTranscoder = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Endpoint"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Endpoint (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EnvironmentCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.EnvironmentCredentials (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.FileSystemCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.FileSystemCredentials (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Firehose"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Firehose ()](#apidoc.element.vogels.AWS.Firehose)
- description and source-code
```javascript
AWS.Firehose = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.GameLift"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.GameLift ()](#apidoc.element.vogels.AWS.GameLift)
- description and source-code
```javascript
AWS.GameLift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Glacier ()](#apidoc.element.vogels.AWS.Glacier)
- description and source-code
```javascript
AWS.Glacier = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.HttpClient ()](#apidoc.element.vogels.AWS.HttpClient)
- description and source-code
```javascript
AWS.HttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpRequest"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.HttpRequest (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest)
- description and source-code
```javascript
function HttpRequest(endpoint, region, customUserAgent) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent(customUserAgent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpResponse"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.HttpResponse ()](#apidoc.element.vogels.AWS.HttpResponse)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IAM"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.IAM ()](#apidoc.element.vogels.AWS.IAM)
- description and source-code
```javascript
AWS.IAM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ImportExport"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ImportExport ()](#apidoc.element.vogels.AWS.ImportExport)
- description and source-code
```javascript
AWS.ImportExport = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Inspector"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Inspector ()](#apidoc.element.vogels.AWS.Inspector)
- description and source-code
```javascript
AWS.Inspector = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Iot"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Iot ()](#apidoc.element.vogels.AWS.Iot)
- description and source-code
```javascript
AWS.Iot = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IotData"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.IotData ()](#apidoc.element.vogels.AWS.IotData)
- description and source-code
```javascript
AWS.IotData = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.KMS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.KMS ()](#apidoc.element.vogels.AWS.KMS)
- description and source-code
```javascript
AWS.KMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Kinesis"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Kinesis ()](#apidoc.element.vogels.AWS.Kinesis)
- description and source-code
```javascript
AWS.Kinesis = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Lambda"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Lambda ()](#apidoc.element.vogels.AWS.Lambda)
- description and source-code
```javascript
AWS.Lambda = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MachineLearning"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.MachineLearning ()](#apidoc.element.vogels.AWS.MachineLearning)
- description and source-code
```javascript
AWS.MachineLearning = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.MarketplaceCommerceAnalytics ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics)
- description and source-code
```javascript
AWS.MarketplaceCommerceAnalytics = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MarketplaceMetering"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.MarketplaceMetering ()](#apidoc.element.vogels.AWS.MarketplaceMetering)
- description and source-code
```javascript
AWS.MarketplaceMetering = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MetadataService"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.MetadataService (options)](#apidoc.element.vogels.AWS.MetadataService)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MobileAnalytics"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.MobileAnalytics ()](#apidoc.element.vogels.AWS.MobileAnalytics)
- description and source-code
```javascript
AWS.MobileAnalytics = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.NodeHttpClient"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.NodeHttpClient ()](#apidoc.element.vogels.AWS.NodeHttpClient)
- description and source-code
```javascript
AWS.NodeHttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.OpsWorks"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.OpsWorks ()](#apidoc.element.vogels.AWS.OpsWorks)
- description and source-code
```javascript
AWS.OpsWorks = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ParamValidator (validation)](#apidoc.element.vogels.AWS.ParamValidator)
- description and source-code
```javascript
function ParamValidator(validation) {
  if (validation === true || validation === undefined) {
    validation = {'min': true};
  }
  this.validation = validation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.RDS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.RDS ()](#apidoc.element.vogels.AWS.RDS)
- description and source-code
```javascript
AWS.RDS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Redshift"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Redshift ()](#apidoc.element.vogels.AWS.Redshift)
- description and source-code
```javascript
AWS.Redshift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Request (service, operation, params)](#apidoc.element.vogels.AWS.Request)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;
  var customUserAgent = service.config.customUserAgent;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region, customUserAgent);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');
  this._haltHandlersOnError = false;

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.ResourceWaiter (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Response"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Response (request)](#apidoc.element.vogels.AWS.Response)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Route53 ()](#apidoc.element.vogels.AWS.Route53)
- description and source-code
```javascript
AWS.Route53 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53Domains"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Route53Domains ()](#apidoc.element.vogels.AWS.Route53Domains)
- description and source-code
```javascript
AWS.Route53Domains = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.S3 ()](#apidoc.element.vogels.AWS.S3)
- description and source-code
```javascript
AWS.S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SAMLCredentials (params)](#apidoc.element.vogels.AWS.SAMLCredentials)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SES"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SES ()](#apidoc.element.vogels.AWS.SES)
- description and source-code
```javascript
AWS.SES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SNS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SNS ()](#apidoc.element.vogels.AWS.SNS)
- description and source-code
```javascript
AWS.SNS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SQS ()](#apidoc.element.vogels.AWS.SQS)
- description and source-code
```javascript
AWS.SQS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SSM"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SSM ()](#apidoc.element.vogels.AWS.SSM)
- description and source-code
```javascript
AWS.SSM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.STS"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.STS ()](#apidoc.element.vogels.AWS.STS)
- description and source-code
```javascript
AWS.STS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SWF"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SWF ()](#apidoc.element.vogels.AWS.SWF)
- description and source-code
```javascript
AWS.SWF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SequentialExecutor ()](#apidoc.element.vogels.AWS.SequentialExecutor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Service (config)](#apidoc.element.vogels.AWS.Service)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SharedIniFileCredentials (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SimpleDB"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.SimpleDB ()](#apidoc.element.vogels.AWS.SimpleDB)
- description and source-code
```javascript
AWS.SimpleDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.StorageGateway"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.StorageGateway ()](#apidoc.element.vogels.AWS.StorageGateway)
- description and source-code
```javascript
AWS.StorageGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Support"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.Support ()](#apidoc.element.vogels.AWS.Support)
- description and source-code
```javascript
AWS.Support = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.TemporaryCredentials (params)](#apidoc.element.vogels.AWS.TemporaryCredentials)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WAF"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.WAF ()](#apidoc.element.vogels.AWS.WAF)
- description and source-code
```javascript
AWS.WAF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.WebIdentityCredentials (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WorkSpaces"></a>[function <span class="apidocSignatureSpan">vogels.</span>AWS.WorkSpaces ()](#apidoc.element.vogels.AWS.WorkSpaces)
- description and source-code
```javascript
AWS.WorkSpaces = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.Set"></a>[function <span class="apidocSignatureSpan">vogels.</span>Set ()](#apidoc.element.vogels.Set)
- description and source-code
```javascript
Set = function () {
  return internals.docClient.createSet.apply(internals.docClient, arguments);
}
```
- example usage
```shell
...
  };

  params.ExpressionAttributeValues = {
    ':inc' : 1,
    ':current' : 2001,
    ':title' : ['The Man'],
    ':firstName' : 'Rob',
    ':tag' : vogels.Set(['Sports', 'Horror'], 'S')
  };

Movie.update({title : 'Movie 0', description : 'This is a description'}, params, function (err, mov) {});
'''

### Deleting
You delete items in DynamoDB using the hashkey of model
...
```

#### <a name="apidoc.element.vogels.createTables"></a>[function <span class="apidocSignatureSpan">vogels.</span>createTables (options, callback)](#apidoc.element.vogels.createTables)
- description and source-code
```javascript
createTables = function (options, callback) {
  if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  callback = callback || _.noop;
  options = options || {};

  return createTables(vogels.models, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.define"></a>[function <span class="apidocSignatureSpan">vogels.</span>define (modelName, config)](#apidoc.element.vogels.define)
- description and source-code
```javascript
define = function (modelName, config) {
  if(_.isFunction(config)) {
    throw new Error('define no longer accepts schema callback, migrate to new api');
  }

  var schema = new Schema(config);

  var compiledTable = internals.compileModel(modelName, schema);

  return compiledTable;
}
```
- example usage
```shell
...
| us-west-1      | US West (N. California)  |
| us-west-2      | US West (Oregon)         |

### Define a Model
Models are defined through the toplevel define method.

'''js
var Account = vogels.define('Account', {
hashKey : 'email',

// add the timestamp attributes (updatedAt, createdAt)
timestamps : true,

schema : {
  email   : Joi.string().email(),
...
```

#### <a name="apidoc.element.vogels.documentClient"></a>[function <span class="apidocSignatureSpan">vogels.</span>documentClient (docClient)](#apidoc.element.vogels.documentClient)
- description and source-code
```javascript
documentClient = function (docClient) {
  if(docClient) {
    internals.docClient = docClient;
    internals.dynamodb = docClient.service;
    internals.updateDynamoDBDocClientForAllModels(docClient);
  } else {
    internals.loadDocClient();
  }

  return internals.docClient;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.dynamoDriver"></a>[function <span class="apidocSignatureSpan">vogels.</span>dynamoDriver (driver)](#apidoc.element.vogels.dynamoDriver)
- description and source-code
```javascript
dynamoDriver = function (driver) {
  if(driver) {
    internals.dynamodb = driver;

    var docClient = internals.loadDocClient(driver);
    internals.updateDynamoDBDocClientForAllModels(docClient);
  } else {
    internals.dynamodb = internals.dynamodb || new vogels.AWS.DynamoDB({apiVersion: '2012-08-10'});
  }

  return internals.dynamodb;
}
```
- example usage
```shell
...
You can also pass in a custom instance of the aws-sdk DynamoDB client
'''js
var dynamodb = new AWS.DynamoDB();
Account.config({dynamodb: dynamodb});

// or globally use custom DynamoDB instance
// all defined models will now use this driver
vogels.dynamoDriver(dynamodb);
'''

### Saving Models to DynamoDB
With your models defined, we can start saving them to DynamoDB.

'''js
Account.create({email: 'foo@example.com', name: 'Foo Bar', age: 21}, function (err, acc) {
...
```

#### <a name="apidoc.element.vogels.item"></a>[function <span class="apidocSignatureSpan">vogels.</span>item (attrs, table)](#apidoc.element.vogels.item)
- description and source-code
```javascript
item = function (attrs, table) {
  events.EventEmitter.call(this);

  this.table = table;

  this.set(attrs || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.model"></a>[function <span class="apidocSignatureSpan">vogels.</span>model (name, model)](#apidoc.element.vogels.model)
- description and source-code
```javascript
model = function (name, model) {
  if(model) {
    internals.addModel(name, model);
  }

  return vogels.models[name] || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.parallelScan"></a>[function <span class="apidocSignatureSpan">vogels.</span>parallelScan (table, serializer, totalSegments)](#apidoc.element.vogels.parallelScan)
- description and source-code
```javascript
parallelScan = function (table, serializer, totalSegments) {
  Scan.call(this, table, serializer);

  this.totalSegments = totalSegments;
}
```
- example usage
```shell
...
The only difference is you must provide the total number of segments

**Caution** you can easily consume all your provisioned throughput with this api

'''js
var totalSegments = 8;

Account.parallelScan(totalSegments)
.where('age').gte(18)
.attributes('age')
.exec(callback);

// Load All accounts
Account
.parallelScan(totalSegments)
...
```

#### <a name="apidoc.element.vogels.query"></a>[function <span class="apidocSignatureSpan">vogels.</span>query (hashKey, table, serializer)](#apidoc.element.vogels.query)
- description and source-code
```javascript
query = function (hashKey, table, serializer) {
  this.hashKey = hashKey;
  this.table = table;
  this.serializer = serializer;

  this.options = {loadAll: false};
  this.request = {};
}
```
- example usage
```shell
...
### Query
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.reset"></a>[function <span class="apidocSignatureSpan">vogels.</span>reset ()](#apidoc.element.vogels.reset)
- description and source-code
```javascript
reset = function () {
  vogels.models = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.scan"></a>[function <span class="apidocSignatureSpan">vogels.</span>scan (table, serializer)](#apidoc.element.vogels.scan)
- description and source-code
```javascript
scan = function (table, serializer) {
  this.table = table;
  this.serializer = serializer;
  this.options = {loadAll: false};

  this.request = {};
}
```
- example usage
```shell
...

### Scan
Vogels provides a flexible and chainable api for scanning over all your items
This api is very similar to the query api.

'''js
// scan all accounts, returning the first page or results
Account.scan().exec(callback);

// scan all accounts, this time loading all results
// note this will potentially make several calls to DynamoDB
// in order to load all results
Account
.scan()
.loadAll()
...
```

#### <a name="apidoc.element.vogels.schema"></a>[function <span class="apidocSignatureSpan">vogels.</span>schema (config)](#apidoc.element.vogels.schema)
- description and source-code
```javascript
schema = function (config) {
  this.secondaryIndexes = {};
  this.globalIndexes = {};

  var context = {hashKey : config.hashKey};

  var self = this;
  Joi.validate(config, internals.configSchema, { context: context }, function (err, data) {
    if(err) {
      var msg = 'Invalid table schema, check your config ';
      throw new Error(msg + err.annotate());
    }

    self.hashKey    = data.hashKey;
    self.rangeKey   = data.rangeKey;
    self.tableName  = data.tableName;
    self.timestamps = data.timestamps;
    self.createdAt  = data.createdAt;
    self.updatedAt  = data.updatedAt;

    if(data.indexes) {
      self.globalIndexes    = _.chain(data.indexes).filter({ type: 'global' }).indexBy('name').value();
      self.secondaryIndexes = _.chain(data.indexes).filter({ type: 'local' }).indexBy('name').value();
    }

    if(data.schema) {
      self._modelSchema    = _.isPlainObject(data.schema) ? Joi.object().keys(data.schema) : data.schema;
    } else {
      self._modelSchema = Joi.object();
    }

    if(self.timestamps) {
      var valids = {};
      var createdAtParamName = 'createdAt';
      var updatedAtParamName = 'updatedAt';

      if(self.createdAt) {
        if(_.isString(self.createdAt)) {
          createdAtParamName = self.createdAt;
        }
      }

      if(self.updatedAt) {
        if(_.isString(self.updatedAt)) {
          updatedAtParamName = self.updatedAt;
        }
      }

      if(self.createdAt !== false) {
        valids[createdAtParamName] = Joi.date();
      }

      if(self.updatedAt !== false) {
        valids[updatedAtParamName] = Joi.date();
      }

      var extended = self._modelSchema.keys(valids);

      self._modelSchema = extended;
    }

    self._modelDatatypes = internals.parseDynamoTypes(self._modelSchema.describe());
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.table"></a>[function <span class="apidocSignatureSpan">vogels.</span>table (name, schema, serializer, docClient, logger)](#apidoc.element.vogels.table)
- description and source-code
```javascript
table = function (name, schema, serializer, docClient, logger) {
  this.config = {name : name};
  this.schema = schema;
  this.serializer = serializer;
  this.docClient = docClient;
  this.log = logger;

  this._before = new EventEmitter();
  this.before = this._before.on.bind(this._before);

  this._after= new EventEmitter();
  this.after = this._after.on.bind(this._after);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS"></a>[module vogels.AWS](#apidoc.module.vogels.AWS)

#### <a name="apidoc.element.vogels.AWS.ACM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ACM ()](#apidoc.element.vogels.AWS.ACM)
- description and source-code
```javascript
ACM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.APIGateway"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>APIGateway ()](#apidoc.element.vogels.AWS.APIGateway)
- description and source-code
```javascript
APIGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.AutoScaling"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>AutoScaling ()](#apidoc.element.vogels.AWS.AutoScaling)
- description and source-code
```javascript
AutoScaling = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFormation"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFormation ()](#apidoc.element.vogels.AWS.CloudFormation)
- description and source-code
```javascript
CloudFormation = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFront ()](#apidoc.element.vogels.AWS.CloudFront)
- description and source-code
```javascript
CloudFront = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudHSM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudHSM ()](#apidoc.element.vogels.AWS.CloudHSM)
- description and source-code
```javascript
CloudHSM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearch"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearch ()](#apidoc.element.vogels.AWS.CloudSearch)
- description and source-code
```javascript
CloudSearch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearchDomain ()](#apidoc.element.vogels.AWS.CloudSearchDomain)
- description and source-code
```javascript
CloudSearchDomain = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudTrail"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudTrail ()](#apidoc.element.vogels.AWS.CloudTrail)
- description and source-code
```javascript
CloudTrail = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatch"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatch ()](#apidoc.element.vogels.AWS.CloudWatch)
- description and source-code
```javascript
CloudWatch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatchEvents"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchEvents ()](#apidoc.element.vogels.AWS.CloudWatchEvents)
- description and source-code
```javascript
CloudWatchEvents = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatchLogs"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchLogs ()](#apidoc.element.vogels.AWS.CloudWatchLogs)
- description and source-code
```javascript
CloudWatchLogs = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodeCommit"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeCommit ()](#apidoc.element.vogels.AWS.CodeCommit)
- description and source-code
```javascript
CodeCommit = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodeDeploy"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeDeploy ()](#apidoc.element.vogels.AWS.CodeDeploy)
- description and source-code
```javascript
CodeDeploy = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodePipeline"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CodePipeline ()](#apidoc.element.vogels.AWS.CodePipeline)
- description and source-code
```javascript
CodePipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentity ()](#apidoc.element.vogels.AWS.CognitoIdentity)
- description and source-code
```javascript
CognitoIdentity = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoSync"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoSync ()](#apidoc.element.vogels.AWS.CognitoSync)
- description and source-code
```javascript
CognitoSync = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Config (options)](#apidoc.element.vogels.AWS.Config)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ConfigService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ConfigService ()](#apidoc.element.vogels.AWS.ConfigService)
- description and source-code
```javascript
ConfigService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CredentialProviderChain"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Credentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Credentials ()](#apidoc.element.vogels.AWS.Credentials)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DMS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DMS ()](#apidoc.element.vogels.AWS.DMS)
- description and source-code
```javascript
DMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DataPipeline"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DataPipeline ()](#apidoc.element.vogels.AWS.DataPipeline)
- description and source-code
```javascript
DataPipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DeviceFarm"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DeviceFarm ()](#apidoc.element.vogels.AWS.DeviceFarm)
- description and source-code
```javascript
DeviceFarm = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DirectConnect"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectConnect ()](#apidoc.element.vogels.AWS.DirectConnect)
- description and source-code
```javascript
DirectConnect = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DirectoryService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectoryService ()](#apidoc.element.vogels.AWS.DirectoryService)
- description and source-code
```javascript
DirectoryService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDB ()](#apidoc.element.vogels.AWS.DynamoDB)
- description and source-code
```javascript
DynamoDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
...

'''js
Account.config({tableName: 'AccountsTable'});
'''

You can also pass in a custom instance of the aws-sdk DynamoDB client
'''js
var dynamodb = new AWS.DynamoDB();
Account.config({dynamodb: dynamodb});

// or globally use custom DynamoDB instance
// all defined models will now use this driver
vogels.dynamoDriver(dynamodb);
'''
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDBStreams"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDBStreams ()](#apidoc.element.vogels.AWS.DynamoDBStreams)
- description and source-code
```javascript
DynamoDBStreams = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2 ()](#apidoc.element.vogels.AWS.EC2)
- description and source-code
```javascript
EC2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2MetadataCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ECR"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ECR ()](#apidoc.element.vogels.AWS.ECR)
- description and source-code
```javascript
ECR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ECS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ECS ()](#apidoc.element.vogels.AWS.ECS)
- description and source-code
```javascript
ECS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EFS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EFS ()](#apidoc.element.vogels.AWS.EFS)
- description and source-code
```javascript
EFS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ELB"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ELB ()](#apidoc.element.vogels.AWS.ELB)
- description and source-code
```javascript
ELB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EMR"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EMR ()](#apidoc.element.vogels.AWS.EMR)
- description and source-code
```javascript
EMR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ES"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ES ()](#apidoc.element.vogels.AWS.ES)
- description and source-code
```javascript
ES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElastiCache"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ElastiCache ()](#apidoc.element.vogels.AWS.ElastiCache)
- description and source-code
```javascript
ElastiCache = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElasticBeanstalk"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticBeanstalk ()](#apidoc.element.vogels.AWS.ElasticBeanstalk)
- description and source-code
```javascript
ElasticBeanstalk = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElasticTranscoder"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticTranscoder ()](#apidoc.element.vogels.AWS.ElasticTranscoder)
- description and source-code
```javascript
ElasticTranscoder = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Endpoint"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EnvironmentCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.FileSystemCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Firehose"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Firehose ()](#apidoc.element.vogels.AWS.Firehose)
- description and source-code
```javascript
Firehose = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.GameLift"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>GameLift ()](#apidoc.element.vogels.AWS.GameLift)
- description and source-code
```javascript
GameLift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Glacier ()](#apidoc.element.vogels.AWS.Glacier)
- description and source-code
```javascript
Glacier = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpClient ()](#apidoc.element.vogels.AWS.HttpClient)
- description and source-code
```javascript
HttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpRequest"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpRequest (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest)
- description and source-code
```javascript
function HttpRequest(endpoint, region, customUserAgent) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent(customUserAgent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpResponse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpResponse ()](#apidoc.element.vogels.AWS.HttpResponse)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IAM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>IAM ()](#apidoc.element.vogels.AWS.IAM)
- description and source-code
```javascript
IAM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ImportExport"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ImportExport ()](#apidoc.element.vogels.AWS.ImportExport)
- description and source-code
```javascript
ImportExport = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Inspector"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Inspector ()](#apidoc.element.vogels.AWS.Inspector)
- description and source-code
```javascript
Inspector = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Iot"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Iot ()](#apidoc.element.vogels.AWS.Iot)
- description and source-code
```javascript
Iot = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IotData"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>IotData ()](#apidoc.element.vogels.AWS.IotData)
- description and source-code
```javascript
IotData = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.KMS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>KMS ()](#apidoc.element.vogels.AWS.KMS)
- description and source-code
```javascript
KMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Kinesis"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Kinesis ()](#apidoc.element.vogels.AWS.Kinesis)
- description and source-code
```javascript
Kinesis = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Lambda"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Lambda ()](#apidoc.element.vogels.AWS.Lambda)
- description and source-code
```javascript
Lambda = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MachineLearning"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MachineLearning ()](#apidoc.element.vogels.AWS.MachineLearning)
- description and source-code
```javascript
MachineLearning = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceCommerceAnalytics ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics)
- description and source-code
```javascript
MarketplaceCommerceAnalytics = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MarketplaceMetering"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceMetering ()](#apidoc.element.vogels.AWS.MarketplaceMetering)
- description and source-code
```javascript
MarketplaceMetering = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MetadataService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MetadataService (options)](#apidoc.element.vogels.AWS.MetadataService)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MobileAnalytics"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MobileAnalytics ()](#apidoc.element.vogels.AWS.MobileAnalytics)
- description and source-code
```javascript
MobileAnalytics = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.NodeHttpClient"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>NodeHttpClient ()](#apidoc.element.vogels.AWS.NodeHttpClient)
- description and source-code
```javascript
NodeHttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.OpsWorks"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>OpsWorks ()](#apidoc.element.vogels.AWS.OpsWorks)
- description and source-code
```javascript
OpsWorks = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ParamValidator (validation)](#apidoc.element.vogels.AWS.ParamValidator)
- description and source-code
```javascript
function ParamValidator(validation) {
  if (validation === true || validation === undefined) {
    validation = {'min': true};
  }
  this.validation = validation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.RDS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>RDS ()](#apidoc.element.vogels.AWS.RDS)
- description and source-code
```javascript
RDS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Redshift"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Redshift ()](#apidoc.element.vogels.AWS.Redshift)
- description and source-code
```javascript
Redshift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Request (service, operation, params)](#apidoc.element.vogels.AWS.Request)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;
  var customUserAgent = service.config.customUserAgent;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region, customUserAgent);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');
  this._haltHandlersOnError = false;

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Response"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Response (request)](#apidoc.element.vogels.AWS.Response)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53 ()](#apidoc.element.vogels.AWS.Route53)
- description and source-code
```javascript
Route53 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53Domains"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53Domains ()](#apidoc.element.vogels.AWS.Route53Domains)
- description and source-code
```javascript
Route53Domains = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>S3 ()](#apidoc.element.vogels.AWS.S3)
- description and source-code
```javascript
S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SAMLCredentials (params)](#apidoc.element.vogels.AWS.SAMLCredentials)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SES"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SES ()](#apidoc.element.vogels.AWS.SES)
- description and source-code
```javascript
SES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SNS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SNS ()](#apidoc.element.vogels.AWS.SNS)
- description and source-code
```javascript
SNS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SQS ()](#apidoc.element.vogels.AWS.SQS)
- description and source-code
```javascript
SQS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SSM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SSM ()](#apidoc.element.vogels.AWS.SSM)
- description and source-code
```javascript
SSM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.STS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>STS ()](#apidoc.element.vogels.AWS.STS)
- description and source-code
```javascript
STS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SWF"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SWF ()](#apidoc.element.vogels.AWS.SWF)
- description and source-code
```javascript
SWF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SequentialExecutor ()](#apidoc.element.vogels.AWS.SequentialExecutor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Service (config)](#apidoc.element.vogels.AWS.Service)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SimpleDB"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SimpleDB ()](#apidoc.element.vogels.AWS.SimpleDB)
- description and source-code
```javascript
SimpleDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.StorageGateway"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>StorageGateway ()](#apidoc.element.vogels.AWS.StorageGateway)
- description and source-code
```javascript
StorageGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Support"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Support ()](#apidoc.element.vogels.AWS.Support)
- description and source-code
```javascript
Support = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>TemporaryCredentials (params)](#apidoc.element.vogels.AWS.TemporaryCredentials)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WAF"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>WAF ()](#apidoc.element.vogels.AWS.WAF)
- description and source-code
```javascript
WAF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WorkSpaces"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>WorkSpaces ()](#apidoc.element.vogels.AWS.WorkSpaces)
- description and source-code
```javascript
WorkSpaces = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.apiLoader"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>apiLoader (svc, version)](#apidoc.element.vogels.AWS.apiLoader)
- description and source-code
```javascript
function load(svc, version) {
  buildServiceMap();
  svc = serviceIdentifier(svc);
  if (version === 'latest') version = null;
  version = version || serviceMap[svc].versions[serviceMap[svc].versions.length - 1];
  if (!serviceMap[svc]) return null;

  var api = require(serviceFile(svc, version));

  // Try to load paginators
  if (fs.existsSync(paginatorsFile(svc, version))) {
    var paginators = require(paginatorsFile(svc, version));
    api.paginators = paginators.pagination;
  }

  // Try to load waiters
  if (fs.existsSync(waitersFile(svc, version))) {
    var waiters = require(waitersFile(svc, version));
    api.waiters = waiters.waiters;
  }

  return api;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ACM"></a>[module vogels.AWS.ACM](#apidoc.module.vogels.AWS.ACM)

#### <a name="apidoc.element.vogels.AWS.ACM.ACM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ACM ()](#apidoc.element.vogels.AWS.ACM.ACM)
- description and source-code
```javascript
ACM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ACM.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ACM.</span>__super__ (config)](#apidoc.element.vogels.AWS.ACM.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ACM.prototype"></a>[module vogels.AWS.ACM.prototype](#apidoc.module.vogels.AWS.ACM.prototype)

#### <a name="apidoc.element.vogels.AWS.ACM.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ACM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ACM.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.APIGateway"></a>[module vogels.AWS.APIGateway](#apidoc.module.vogels.AWS.APIGateway)

#### <a name="apidoc.element.vogels.AWS.APIGateway.APIGateway"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>APIGateway ()](#apidoc.element.vogels.AWS.APIGateway.APIGateway)
- description and source-code
```javascript
APIGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.APIGateway.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.</span>__super__ (config)](#apidoc.element.vogels.AWS.APIGateway.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.APIGateway.prototype"></a>[module vogels.AWS.APIGateway.prototype](#apidoc.module.vogels.AWS.APIGateway.prototype)

#### <a name="apidoc.element.vogels.AWS.APIGateway.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.APIGateway.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.APIGateway.prototype.setAcceptHeader"></a>[function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.prototype.</span>setAcceptHeader (req)](#apidoc.element.vogels.AWS.APIGateway.prototype.setAcceptHeader)
- description and source-code
```javascript
function setAcceptHeader(req) {
  var httpRequest = req.httpRequest;
  httpRequest.headers['Accept'] = 'application/json';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.APIGateway.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.APIGateway.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.APIGateway.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.addListener('build', this.setAcceptHeader);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.AutoScaling"></a>[module vogels.AWS.AutoScaling](#apidoc.module.vogels.AWS.AutoScaling)

#### <a name="apidoc.element.vogels.AWS.AutoScaling.AutoScaling"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>AutoScaling ()](#apidoc.element.vogels.AWS.AutoScaling.AutoScaling)
- description and source-code
```javascript
AutoScaling = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.AutoScaling.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.</span>__super__ (config)](#apidoc.element.vogels.AWS.AutoScaling.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.AutoScaling.prototype"></a>[module vogels.AWS.AutoScaling.prototype](#apidoc.module.vogels.AWS.AutoScaling.prototype)

#### <a name="apidoc.element.vogels.AWS.AutoScaling.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.AutoScaling.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.AutoScaling.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudFormation"></a>[module vogels.AWS.CloudFormation](#apidoc.module.vogels.AWS.CloudFormation)

#### <a name="apidoc.element.vogels.AWS.CloudFormation.CloudFormation"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFormation ()](#apidoc.element.vogels.AWS.CloudFormation.CloudFormation)
- description and source-code
```javascript
CloudFormation = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFormation.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudFormation.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudFormation.prototype"></a>[module vogels.AWS.CloudFormation.prototype](#apidoc.module.vogels.AWS.CloudFormation.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudFormation.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFormation.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudFormation.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudFront"></a>[module vogels.AWS.CloudFront](#apidoc.module.vogels.AWS.CloudFront)

#### <a name="apidoc.element.vogels.AWS.CloudFront.CloudFront"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudFront ()](#apidoc.element.vogels.AWS.CloudFront.CloudFront)
- description and source-code
```javascript
CloudFront = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront.Signer"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>Signer (keyPairId, privateKey)](#apidoc.element.vogels.AWS.CloudFront.Signer)
- description and source-code
```javascript
function Signer(keyPairId, privateKey) {
    if (keyPairId === void 0 || privateKey === void 0) {
        throw new Error('A key pair ID and private key are required');
    }

    this.keyPairId = keyPairId;
    this.privateKey = privateKey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudFront.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudFront.Signer.prototype"></a>[module vogels.AWS.CloudFront.Signer.prototype](#apidoc.module.vogels.AWS.CloudFront.Signer.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudFront.Signer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.Signer.prototype.</span>constructor (keyPairId, privateKey)](#apidoc.element.vogels.AWS.CloudFront.Signer.prototype.constructor)
- description and source-code
```javascript
function Signer(keyPairId, privateKey) {
    if (keyPairId === void 0 || privateKey === void 0) {
        throw new Error('A key pair ID and private key are required');
    }

    this.keyPairId = keyPairId;
    this.privateKey = privateKey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront.Signer.prototype.getSignedCookie"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.Signer.prototype.</span>getSignedCookie (options, cb)](#apidoc.element.vogels.AWS.CloudFront.Signer.prototype.getSignedCookie)
- description and source-code
```javascript
getSignedCookie = function (options, cb) {
    var signatureHash = 'policy' in options
        ? signWithCustomPolicy(options.policy, this.keyPairId, this.privateKey)
        : signWithCannedPolicy(options.url, options.expires, this.keyPairId, this.privateKey);

    var cookieHash = {};
    for (var key in signatureHash) {
        if (signatureHash.hasOwnProperty(key)) {
            cookieHash['CloudFront-' + key] = signatureHash[key];
        }
    }

    return handleSuccess(cookieHash, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront.Signer.prototype.getSignedUrl"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.Signer.prototype.</span>getSignedUrl (options, cb)](#apidoc.element.vogels.AWS.CloudFront.Signer.prototype.getSignedUrl)
- description and source-code
```javascript
getSignedUrl = function (options, cb) {
    try {
        var resource = getResource(options.url);
    } catch (err) {
        return handleError(err, cb);
    }

    var parsedUrl = url.parse(options.url, true),
        signatureHash = options.hasOwnProperty('policy')
            ? signWithCustomPolicy(options.policy, this.keyPairId, this.privateKey)
            : signWithCannedPolicy(resource, options.expires, this.keyPairId, this.privateKey);

    parsedUrl.search = null;
    for (var key in signatureHash) {
        if (signatureHash.hasOwnProperty(key)) {
            parsedUrl.query[key] = signatureHash[key];
        }
    }

    try {
        var signedUrl = determineScheme(options.url) === 'rtmp'
                ? getRtmpUrl(url.format(parsedUrl))
                : url.format(parsedUrl);
    } catch (err) {
        return handleError(err, cb);
    }

    return handleSuccess(signedUrl, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudFront.prototype"></a>[module vogels.AWS.CloudFront.prototype](#apidoc.module.vogels.AWS.CloudFront.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudFront.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudFront.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudFront.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudFront.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.CloudFront.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.addListener('extractData', AWS.util.hoistPayloadMember);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudHSM"></a>[module vogels.AWS.CloudHSM](#apidoc.module.vogels.AWS.CloudHSM)

#### <a name="apidoc.element.vogels.AWS.CloudHSM.CloudHSM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudHSM ()](#apidoc.element.vogels.AWS.CloudHSM.CloudHSM)
- description and source-code
```javascript
CloudHSM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudHSM.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudHSM.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudHSM.prototype"></a>[module vogels.AWS.CloudHSM.prototype](#apidoc.module.vogels.AWS.CloudHSM.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudHSM.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudHSM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudHSM.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudSearch"></a>[module vogels.AWS.CloudSearch](#apidoc.module.vogels.AWS.CloudSearch)

#### <a name="apidoc.element.vogels.AWS.CloudSearch.CloudSearch"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearch ()](#apidoc.element.vogels.AWS.CloudSearch.CloudSearch)
- description and source-code
```javascript
CloudSearch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearch.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudSearch.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudSearch.prototype"></a>[module vogels.AWS.CloudSearch.prototype](#apidoc.module.vogels.AWS.CloudSearch.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudSearch.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearch.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudSearch.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudSearchDomain"></a>[module vogels.AWS.CloudSearchDomain](#apidoc.module.vogels.AWS.CloudSearchDomain)

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.CloudSearchDomain"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudSearchDomain ()](#apidoc.element.vogels.AWS.CloudSearchDomain.CloudSearchDomain)
- description and source-code
```javascript
CloudSearchDomain = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudSearchDomain.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudSearchDomain.prototype"></a>[module vogels.AWS.CloudSearchDomain.prototype](#apidoc.module.vogels.AWS.CloudSearchDomain.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.removeListener('validate',
    AWS.EventListeners.Core.VALIDATE_CREDENTIALS
  );
  request.onAsync('validate', this.validateCredentials);
  request.addListener('validate', this.updateRegion);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.prototype.updateRegion"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>updateRegion (request)](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.updateRegion)
- description and source-code
```javascript
function updateRegion(request) {
  var endpoint = request.httpRequest.endpoint.hostname;
  var zones = endpoint.split('.');
  request.httpRequest.region = zones[1] || request.httpRequest.region;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.prototype.validateCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>validateCredentials (req, done)](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.validateCredentials)
- description and source-code
```javascript
validateCredentials = function (req, done) {
  if (!req.service.api.signatureVersion) return done(); // none
  req.service.config.getCredentials(function(err) {
    if (err) {
      req.removeListener('sign', AWS.EventListeners.Core.SIGN);
    }
    done();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudSearchDomain.prototype.validateService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudSearchDomain.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.CloudSearchDomain.prototype.validateService)
- description and source-code
```javascript
function validateService() {
  if (!this.config.endpoint || this.config.endpoint.indexOf('{') >= 0) {
    var msg = 'AWS.CloudSearchDomain requires an explicit ' +
              ''endpoint\' configuration option.';
    throw AWS.util.error(new Error(),
      {name: 'InvalidEndpoint', message: msg});
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudTrail"></a>[module vogels.AWS.CloudTrail](#apidoc.module.vogels.AWS.CloudTrail)

#### <a name="apidoc.element.vogels.AWS.CloudTrail.CloudTrail"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudTrail ()](#apidoc.element.vogels.AWS.CloudTrail.CloudTrail)
- description and source-code
```javascript
CloudTrail = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudTrail.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudTrail.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudTrail.prototype"></a>[module vogels.AWS.CloudTrail.prototype](#apidoc.module.vogels.AWS.CloudTrail.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudTrail.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudTrail.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudTrail.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudWatch"></a>[module vogels.AWS.CloudWatch](#apidoc.module.vogels.AWS.CloudWatch)

#### <a name="apidoc.element.vogels.AWS.CloudWatch.CloudWatch"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatch ()](#apidoc.element.vogels.AWS.CloudWatch.CloudWatch)
- description and source-code
```javascript
CloudWatch = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatch.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudWatch.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudWatch.prototype"></a>[module vogels.AWS.CloudWatch.prototype](#apidoc.module.vogels.AWS.CloudWatch.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudWatch.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudWatch.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudWatch.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudWatchEvents"></a>[module vogels.AWS.CloudWatchEvents](#apidoc.module.vogels.AWS.CloudWatchEvents)

#### <a name="apidoc.element.vogels.AWS.CloudWatchEvents.CloudWatchEvents"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchEvents ()](#apidoc.element.vogels.AWS.CloudWatchEvents.CloudWatchEvents)
- description and source-code
```javascript
CloudWatchEvents = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatchEvents.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudWatchEvents.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudWatchEvents.prototype"></a>[module vogels.AWS.CloudWatchEvents.prototype](#apidoc.module.vogels.AWS.CloudWatchEvents.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudWatchEvents.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchEvents.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudWatchEvents.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudWatchLogs"></a>[module vogels.AWS.CloudWatchLogs](#apidoc.module.vogels.AWS.CloudWatchLogs)

#### <a name="apidoc.element.vogels.AWS.CloudWatchLogs.CloudWatchLogs"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CloudWatchLogs ()](#apidoc.element.vogels.AWS.CloudWatchLogs.CloudWatchLogs)
- description and source-code
```javascript
CloudWatchLogs = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CloudWatchLogs.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.</span>__super__ (config)](#apidoc.element.vogels.AWS.CloudWatchLogs.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CloudWatchLogs.prototype"></a>[module vogels.AWS.CloudWatchLogs.prototype](#apidoc.module.vogels.AWS.CloudWatchLogs.prototype)

#### <a name="apidoc.element.vogels.AWS.CloudWatchLogs.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CloudWatchLogs.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CloudWatchLogs.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CodeCommit"></a>[module vogels.AWS.CodeCommit](#apidoc.module.vogels.AWS.CodeCommit)

#### <a name="apidoc.element.vogels.AWS.CodeCommit.CodeCommit"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeCommit ()](#apidoc.element.vogels.AWS.CodeCommit.CodeCommit)
- description and source-code
```javascript
CodeCommit = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodeCommit.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.</span>__super__ (config)](#apidoc.element.vogels.AWS.CodeCommit.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CodeCommit.prototype"></a>[module vogels.AWS.CodeCommit.prototype](#apidoc.module.vogels.AWS.CodeCommit.prototype)

#### <a name="apidoc.element.vogels.AWS.CodeCommit.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CodeCommit.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CodeCommit.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CodeDeploy"></a>[module vogels.AWS.CodeDeploy](#apidoc.module.vogels.AWS.CodeDeploy)

#### <a name="apidoc.element.vogels.AWS.CodeDeploy.CodeDeploy"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CodeDeploy ()](#apidoc.element.vogels.AWS.CodeDeploy.CodeDeploy)
- description and source-code
```javascript
CodeDeploy = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodeDeploy.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.</span>__super__ (config)](#apidoc.element.vogels.AWS.CodeDeploy.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CodeDeploy.prototype"></a>[module vogels.AWS.CodeDeploy.prototype](#apidoc.module.vogels.AWS.CodeDeploy.prototype)

#### <a name="apidoc.element.vogels.AWS.CodeDeploy.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CodeDeploy.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CodeDeploy.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CodePipeline"></a>[module vogels.AWS.CodePipeline](#apidoc.module.vogels.AWS.CodePipeline)

#### <a name="apidoc.element.vogels.AWS.CodePipeline.CodePipeline"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CodePipeline ()](#apidoc.element.vogels.AWS.CodePipeline.CodePipeline)
- description and source-code
```javascript
CodePipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CodePipeline.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.</span>__super__ (config)](#apidoc.element.vogels.AWS.CodePipeline.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CodePipeline.prototype"></a>[module vogels.AWS.CodePipeline.prototype](#apidoc.module.vogels.AWS.CodePipeline.prototype)

#### <a name="apidoc.element.vogels.AWS.CodePipeline.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CodePipeline.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CodePipeline.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CognitoIdentity"></a>[module vogels.AWS.CognitoIdentity](#apidoc.module.vogels.AWS.CognitoIdentity)

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity.CognitoIdentity"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentity ()](#apidoc.element.vogels.AWS.CognitoIdentity.CognitoIdentity)
- description and source-code
```javascript
CognitoIdentity = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.</span>__super__ (config)](#apidoc.element.vogels.AWS.CognitoIdentity.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CognitoIdentity.prototype"></a>[module vogels.AWS.CognitoIdentity.prototype](#apidoc.module.vogels.AWS.CognitoIdentity.prototype)

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity.prototype.getCredentialsForIdentity"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>getCredentialsForIdentity (params, callback)](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.getCredentialsForIdentity)
- description and source-code
```javascript
function getCredentialsForIdentity(params, callback) {
  return this.makeUnauthenticatedRequest('getCredentialsForIdentity', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity.prototype.getId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>getId (params, callback)](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.getId)
- description and source-code
```javascript
function getId(params, callback) {
  return this.makeUnauthenticatedRequest('getId', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentity.prototype.getOpenIdToken"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentity.prototype.</span>getOpenIdToken (params, callback)](#apidoc.element.vogels.AWS.CognitoIdentity.prototype.getOpenIdToken)
- description and source-code
```javascript
function getOpenIdToken(params, callback) {
  return this.makeUnauthenticatedRequest('getOpenIdToken', params, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CognitoIdentityCredentials"></a>[module vogels.AWS.CognitoIdentityCredentials](#apidoc.module.vogels.AWS.CognitoIdentityCredentials)

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.CognitoIdentityCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoIdentityCredentials (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.CognitoIdentityCredentials)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CognitoIdentityCredentials.prototype"></a>[module vogels.AWS.CognitoIdentityCredentials.prototype](#apidoc.module.vogels.AWS.CognitoIdentityCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.cacheId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>cacheId (data)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.cacheId)
- description and source-code
```javascript
function cacheId(data) {
  this.identityId = data.IdentityId;
  this.params.IdentityId = this.identityId;

  // cache this IdentityId in browser localStorage if possible
  if (AWS.util.isBrowser()) {
    this.setStorage('id', data.IdentityId);

    if (this.params.Logins) {
      this.setStorage('providers', Object.keys(this.params.Logins).join(','));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.clearCachedId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>clearCachedId ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.clearCachedId)
- description and source-code
```javascript
function clearCache() {
  this.identityId = null;
  delete this.params.IdentityId;

  var poolId = this.params.IdentityPoolId;
  var loginId = this.params.LoginId || '';
  delete this.storage[this.localStorageKey.id + poolId + loginId];
  delete this.storage[this.localStorageKey.providers + poolId + loginId];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.constructor)
- description and source-code
```javascript
function CognitoIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.data = null;
  this.identityId = null;
  this.loadCachedId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.createClients"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.createClients)
- description and source-code
```javascript
createClients = function () {
  this.webIdentityCredentials = this.webIdentityCredentials ||
    new AWS.WebIdentityCredentials(this.params);
  this.cognito = this.cognito ||
    new AWS.CognitoIdentity({params: this.params});
  this.sts = this.sts || new AWS.STS();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getCredentialsForIdentity"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getCredentialsForIdentity (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getCredentialsForIdentity)
- description and source-code
```javascript
function getCredentialsForIdentity(callback) {
  var self = this;
  self.cognito.getCredentialsForIdentity(function(err, data) {
    if (!err) {
      self.cacheId(data);
      self.data = data;
      self.loadCredentials(self.data, self);
    } else {
      self.clearCachedId();
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getCredentialsFromSTS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getCredentialsFromSTS (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getCredentialsFromSTS)
- description and source-code
```javascript
function getCredentialsFromSTS(callback) {
  var self = this;
  self.cognito.getOpenIdToken(function(err, data) {
    if (!err) {
      self.cacheId(data);
      self.params.WebIdentityToken = data.Token;
      self.webIdentityCredentials.refresh(function(webErr) {
        if (!webErr) {
          self.data = self.webIdentityCredentials.data;
          self.sts.credentialsFrom(self.data, self);
        } else {
          self.clearCachedId();
        }
        callback(webErr);
      });
    } else {
      self.clearCachedId();
      callback(err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getId (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getId)
- description and source-code
```javascript
function getId(callback) {
  var self = this;
  if (typeof self.params.IdentityId === 'string') {
    return callback(null, self.params.IdentityId);
  }

  self.cognito.getId(function(err, data) {
    if (!err && data.IdentityId) {
      self.params.IdentityId = data.IdentityId;
      callback(null, data.IdentityId);
    } else {
      callback(err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getStorage"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>getStorage (key)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.getStorage)
- description and source-code
```javascript
function getStorage(key) {
  return this.storage[this.localStorageKey[key] + this.params.IdentityPoolId + (this.params.LoginId || '')];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.loadCachedId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>loadCachedId ()](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.loadCachedId)
- description and source-code
```javascript
function loadCachedId() {
  var self = this;

  // in the browser we source default IdentityId from localStorage
  if (AWS.util.isBrowser() && !self.params.IdentityId) {
    var id = self.getStorage('id');
    if (id && self.params.Logins) {
      var actualProviders = Object.keys(self.params.Logins);
      var cachedProviders =
        (self.getStorage('providers') || '').split(',');

      // only load ID if at least one provider used this ID before
      var intersect = cachedProviders.filter(function(n) {
        return actualProviders.indexOf(n) !== -1;
      });
      if (intersect.length !== 0) {
        self.params.IdentityId = id;
      }
    } else if (id) {
      self.params.IdentityId = id;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.loadCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>loadCredentials (data, credentials)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.loadCredentials)
- description and source-code
```javascript
function loadCredentials(data, credentials) {
  if (!data || !credentials) return;
  credentials.expired = false;
  credentials.accessKeyId = data.Credentials.AccessKeyId;
  credentials.secretAccessKey = data.Credentials.SecretKey;
  credentials.sessionToken = data.Credentials.SessionToken;
  credentials.expireTime = data.Credentials.Expiration;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  self.createClients();
  self.data = null;
  self.identityId = null;
  self.getId(function(err) {
    if (!err) {
      if (!self.params.RoleArn) {
        self.getCredentialsForIdentity(callback);
      } else {
        self.getCredentialsFromSTS(callback);
      }
    } else {
      self.clearCachedId();
      callback(err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.setStorage"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoIdentityCredentials.prototype.</span>setStorage (key, val)](#apidoc.element.vogels.AWS.CognitoIdentityCredentials.prototype.setStorage)
- description and source-code
```javascript
function setStorage(key, val) {
  try {
    this.storage[this.localStorageKey[key] + this.params.IdentityPoolId + (this.params.LoginId || '')] = val;
  } catch (_) {}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CognitoSync"></a>[module vogels.AWS.CognitoSync](#apidoc.module.vogels.AWS.CognitoSync)

#### <a name="apidoc.element.vogels.AWS.CognitoSync.CognitoSync"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CognitoSync ()](#apidoc.element.vogels.AWS.CognitoSync.CognitoSync)
- description and source-code
```javascript
CognitoSync = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CognitoSync.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.</span>__super__ (config)](#apidoc.element.vogels.AWS.CognitoSync.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CognitoSync.prototype"></a>[module vogels.AWS.CognitoSync.prototype](#apidoc.module.vogels.AWS.CognitoSync.prototype)

#### <a name="apidoc.element.vogels.AWS.CognitoSync.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CognitoSync.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.CognitoSync.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Config"></a>[module vogels.AWS.Config](#apidoc.module.vogels.AWS.Config)

#### <a name="apidoc.element.vogels.AWS.Config.Config"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Config (options)](#apidoc.element.vogels.AWS.Config.Config)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.</span>__super__ ()](#apidoc.element.vogels.AWS.Config.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Config.prototype"></a>[module vogels.AWS.Config.prototype](#apidoc.module.vogels.AWS.Config.prototype)

#### <a name="apidoc.element.vogels.AWS.Config.prototype.clear"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>clear ()](#apidoc.element.vogels.AWS.Config.prototype.clear)
- description and source-code
```javascript
function clear() {
<span class="apidocCodeCommentSpan">  /*jshint forin:false */
</span>  AWS.util.each.call(this, this.keys, function (key) {
    delete this[key];
  });

  // reset credential provider
  this.set('credentials', undefined);
  this.set('credentialProvider', undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.Config.prototype.constructor)
- description and source-code
```javascript
function Config(options) {
  if (options === undefined) options = {};
  options = this.extractCredentials(options);

  AWS.util.each.call(this, this.keys, function (key, value) {
    this.set(key, options[key], value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.extractCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>extractCredentials (options)](#apidoc.element.vogels.AWS.Config.prototype.extractCredentials)
- description and source-code
```javascript
function extractCredentials(options) {
  if (options.accessKeyId && options.secretAccessKey) {
    options = AWS.util.copy(options);
    options.credentials = new AWS.Credentials(options);
  }
  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.getCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>getCredentials (callback)](#apidoc.element.vogels.AWS.Config.prototype.getCredentials)
- description and source-code
```javascript
function getCredentials(callback) {
  var self = this;

  function finish(err) {
    callback(err, err ? null : self.credentials);
  }

  function credError(msg, err) {
    return new AWS.util.error(err || new Error(), {
      code: 'CredentialsError', message: msg
    });
  }

  function getAsyncCredentials() {
    self.credentials.get(function(err) {
      if (err) {
        var msg = 'Could not load credentials from ' +
          self.credentials.constructor.name;
        err = credError(msg, err);
      }
      finish(err);
    });
  }

  function getStaticCredentials() {
    var err = null;
    if (!self.credentials.accessKeyId || !self.credentials.secretAccessKey) {
      err = credError('Missing credentials');
    }
    finish(err);
  }

  if (self.credentials) {
    if (typeof self.credentials.get === 'function') {
      getAsyncCredentials();
    } else { // static credentials
      getStaticCredentials();
    }
  } else if (self.credentialProvider) {
    self.credentialProvider.resolve(function(err, creds) {
      if (err) {
        err = credError('Could not load credentials from any providers', err);
      }
      self.credentials = creds;
      finish(err);
    });
  } else {
    finish(credError('No credentials to load'));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.loadFromPath"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>loadFromPath (path)](#apidoc.element.vogels.AWS.Config.prototype.loadFromPath)
- description and source-code
```javascript
function loadFromPath(path) {
  this.clear();

  var options = JSON.parse(AWS.util.readFileSync(path));
  var fileSystemCreds = new AWS.FileSystemCredentials(path);
  var chain = new AWS.CredentialProviderChain();
  chain.providers.unshift(fileSystemCreds);
  chain.resolve(function (err, creds) {
    if (err) throw err;
    else options.credentials = creds;
  });

  this.constructor(options);

  return this;
}
```
- example usage
```shell
...
    npm install vogels

## Getting Started
First, you need to configure the [AWS SDK][2] with your credentials.

'''js
var vogels = require('vogels');
vogels.AWS.config.loadFromPath('credentials.json');
'''

When running on EC2 its recommended to leverage EC2 IAM roles. If you have configured your instance to use IAM roles, Vogels will
 automatically select these credentials for use in your application, and you do not need to manually provide credentials in any
other format.

'''js
var vogels = require('vogels');
vogels.AWS.config.update({region: "REGION"}); // region must be set
...
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.set"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>set (property, value, defaultValue)](#apidoc.element.vogels.AWS.Config.prototype.set)
- description and source-code
```javascript
function set(property, value, defaultValue) {
  if (value === undefined) {
    if (defaultValue === undefined) {
      defaultValue = this.keys[property];
    }
    if (typeof defaultValue === 'function') {
      this[property] = defaultValue.call(this);
    } else {
      this[property] = defaultValue;
    }
  } else if (property === 'httpOptions' && this[property]) {
    // deep merge httpOptions
    this[property] = AWS.util.merge(this[property], value);
  } else {
    this[property] = value;
  }
}
```
- example usage
```shell
...
    age     : Joi.number(),
  }
});

Account.create({email: 'test@example.com', name : 'Test Account'}, function (err, acc) {
  console.log('created account at', acc.get('created')); // prints created Date

  acc.set({age: 22});

  acc.update(function (err) {
    console.log('updated account age');
  });

});
'''
...
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.update"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.</span>update (options, allowUnknownKeys)](#apidoc.element.vogels.AWS.Config.prototype.update)
- description and source-code
```javascript
function update(options, allowUnknownKeys) {
  allowUnknownKeys = allowUnknownKeys || false;
  options = this.extractCredentials(options);
  AWS.util.each.call(this, options, function (key, value) {
    if (allowUnknownKeys || this.keys.hasOwnProperty(key) ||
        AWS.Service.hasService(key)) {
      this.set(key, value);
    }
  });
}
```
- example usage
```shell
...
vogels.AWS.config.loadFromPath('credentials.json');
'''

When running on EC2 its recommended to leverage EC2 IAM roles. If you have configured your instance to use IAM roles, Vogels will
 automatically select these credentials for use in your application, and you do not need to manually provide credentials in any
other format.

'''js
var vogels = require('vogels');
vogels.AWS.config.update({region: "REGION"}); // region must be set
'''

You can also directly pass in your access key id, secret and region.
  * Its recommend you not hard-code credentials inside an application. Use this method only for small personal scripts or for testing
 purposes.

'''js
var vogels = require('vogels');
...
```



# <a name="apidoc.module.vogels.AWS.Config.prototype.keys"></a>[module vogels.AWS.Config.prototype.keys](#apidoc.module.vogels.AWS.Config.prototype.keys)

#### <a name="apidoc.element.vogels.AWS.Config.prototype.keys.credentialProvider"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>credentialProvider ()](#apidoc.element.vogels.AWS.Config.prototype.keys.credentialProvider)
- description and source-code
```javascript
credentialProvider = function () {
  return new AWS.CredentialProviderChain();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.keys.credentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>credentials ()](#apidoc.element.vogels.AWS.Config.prototype.keys.credentials)
- description and source-code
```javascript
credentials = function () {
  var credentials = null;
  new AWS.CredentialProviderChain([
    function () { return new AWS.EnvironmentCredentials('AWS'); },
    function () { return new AWS.EnvironmentCredentials('AMAZON'); },
    function () { return new AWS.SharedIniFileCredentials(); }
  ]).resolve(function(err, creds) {
    if (!err) credentials = creds;
  });
  return credentials;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Config.prototype.keys.region"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Config.prototype.keys.</span>region ()](#apidoc.element.vogels.AWS.Config.prototype.keys.region)
- description and source-code
```javascript
region = function () {
  return process.env.AWS_REGION || process.env.AMAZON_REGION;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ConfigService"></a>[module vogels.AWS.ConfigService](#apidoc.module.vogels.AWS.ConfigService)

#### <a name="apidoc.element.vogels.AWS.ConfigService.ConfigService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ConfigService ()](#apidoc.element.vogels.AWS.ConfigService.ConfigService)
- description and source-code
```javascript
ConfigService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ConfigService.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ConfigService.</span>__super__ (config)](#apidoc.element.vogels.AWS.ConfigService.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ConfigService.prototype"></a>[module vogels.AWS.ConfigService.prototype](#apidoc.module.vogels.AWS.ConfigService.prototype)

#### <a name="apidoc.element.vogels.AWS.ConfigService.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ConfigService.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ConfigService.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CredentialProviderChain"></a>[module vogels.AWS.CredentialProviderChain](#apidoc.module.vogels.AWS.CredentialProviderChain)

#### <a name="apidoc.element.vogels.AWS.CredentialProviderChain.CredentialProviderChain"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>CredentialProviderChain (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain.CredentialProviderChain)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CredentialProviderChain.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.</span>__super__ ()](#apidoc.element.vogels.AWS.CredentialProviderChain.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.CredentialProviderChain.prototype"></a>[module vogels.AWS.CredentialProviderChain.prototype](#apidoc.module.vogels.AWS.CredentialProviderChain.prototype)

#### <a name="apidoc.element.vogels.AWS.CredentialProviderChain.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.prototype.</span>constructor (providers)](#apidoc.element.vogels.AWS.CredentialProviderChain.prototype.constructor)
- description and source-code
```javascript
function CredentialProviderChain(providers) {
  if (providers) {
    this.providers = providers;
  } else {
    this.providers = AWS.CredentialProviderChain.defaultProviders.slice(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.CredentialProviderChain.prototype.resolve"></a>[function <span class="apidocSignatureSpan">vogels.AWS.CredentialProviderChain.prototype.</span>resolve (callback)](#apidoc.element.vogels.AWS.CredentialProviderChain.prototype.resolve)
- description and source-code
```javascript
function resolve(callback) {
  if (this.providers.length === 0) {
    callback(new Error('No providers'));
    return this;
  }

  var index = 0;
  var providers = this.providers.slice(0);

  function resolveNext(err, creds) {
    if ((!err && creds) || index === providers.length) {
      callback(err, creds);
      return;
    }

    var provider = providers[index++];
    if (typeof provider === 'function') {
      creds = provider.call();
    } else {
      creds = provider;
    }

    if (creds.get) {
      creds.get(function(getErr) {
        resolveNext(getErr, getErr ? null : creds);
      });
    } else {
      resolveNext(null, creds);
    }
  }

  resolveNext();
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Credentials"></a>[module vogels.AWS.Credentials](#apidoc.module.vogels.AWS.Credentials)

#### <a name="apidoc.element.vogels.AWS.Credentials.Credentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Credentials ()](#apidoc.element.vogels.AWS.Credentials.Credentials)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Credentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Credentials.</span>__super__ ()](#apidoc.element.vogels.AWS.Credentials.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Credentials.prototype"></a>[module vogels.AWS.Credentials.prototype](#apidoc.module.vogels.AWS.Credentials.prototype)

#### <a name="apidoc.element.vogels.AWS.Credentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Credentials.prototype.constructor)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Credentials.prototype.get"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>get (callback)](#apidoc.element.vogels.AWS.Credentials.prototype.get)
- description and source-code
```javascript
function get(callback) {
  var self = this;
  if (this.needsRefresh()) {
    this.refresh(function(err) {
      if (!err) self.expired = false; // reset expired flag
      if (callback) callback(err);
    });
  } else if (callback) {
    callback();
  }
}
```
- example usage
```shell
...
'''

### Saving Models to DynamoDB
With your models defined, we can start saving them to DynamoDB.

'''js
Account.create({email: 'foo@example.com', name: 'Foo Bar', age: 21}, function (err, acc) {
  console.log('created account in DynamoDB', acc.get('email'));
});
'''

You can also first instantiate a model and then save it.

'''js
var acc = new Account({email: 'test@example.com', name: 'Test Example'});
...
```

#### <a name="apidoc.element.vogels.AWS.Credentials.prototype.needsRefresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>needsRefresh ()](#apidoc.element.vogels.AWS.Credentials.prototype.needsRefresh)
- description and source-code
```javascript
function needsRefresh() {
  var currentTime = AWS.util.date.getDate().getTime();
  var adjustedTime = new Date(currentTime + this.expiryWindow * 1000);

  if (this.expireTime && adjustedTime > this.expireTime) {
    return true;
  } else {
    return this.expired || !this.accessKeyId || !this.secretAccessKey;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Credentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Credentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.Credentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  this.expired = false;
  callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DMS"></a>[module vogels.AWS.DMS](#apidoc.module.vogels.AWS.DMS)

#### <a name="apidoc.element.vogels.AWS.DMS.DMS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DMS ()](#apidoc.element.vogels.AWS.DMS.DMS)
- description and source-code
```javascript
DMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DMS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DMS.</span>__super__ (config)](#apidoc.element.vogels.AWS.DMS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DMS.prototype"></a>[module vogels.AWS.DMS.prototype](#apidoc.module.vogels.AWS.DMS.prototype)

#### <a name="apidoc.element.vogels.AWS.DMS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DMS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DMS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DataPipeline"></a>[module vogels.AWS.DataPipeline](#apidoc.module.vogels.AWS.DataPipeline)

#### <a name="apidoc.element.vogels.AWS.DataPipeline.DataPipeline"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DataPipeline ()](#apidoc.element.vogels.AWS.DataPipeline.DataPipeline)
- description and source-code
```javascript
DataPipeline = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DataPipeline.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.</span>__super__ (config)](#apidoc.element.vogels.AWS.DataPipeline.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DataPipeline.prototype"></a>[module vogels.AWS.DataPipeline.prototype](#apidoc.module.vogels.AWS.DataPipeline.prototype)

#### <a name="apidoc.element.vogels.AWS.DataPipeline.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DataPipeline.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DataPipeline.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DeviceFarm"></a>[module vogels.AWS.DeviceFarm](#apidoc.module.vogels.AWS.DeviceFarm)

#### <a name="apidoc.element.vogels.AWS.DeviceFarm.DeviceFarm"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DeviceFarm ()](#apidoc.element.vogels.AWS.DeviceFarm.DeviceFarm)
- description and source-code
```javascript
DeviceFarm = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DeviceFarm.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.</span>__super__ (config)](#apidoc.element.vogels.AWS.DeviceFarm.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DeviceFarm.prototype"></a>[module vogels.AWS.DeviceFarm.prototype](#apidoc.module.vogels.AWS.DeviceFarm.prototype)

#### <a name="apidoc.element.vogels.AWS.DeviceFarm.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DeviceFarm.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DeviceFarm.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DirectConnect"></a>[module vogels.AWS.DirectConnect](#apidoc.module.vogels.AWS.DirectConnect)

#### <a name="apidoc.element.vogels.AWS.DirectConnect.DirectConnect"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectConnect ()](#apidoc.element.vogels.AWS.DirectConnect.DirectConnect)
- description and source-code
```javascript
DirectConnect = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DirectConnect.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.</span>__super__ (config)](#apidoc.element.vogels.AWS.DirectConnect.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DirectConnect.prototype"></a>[module vogels.AWS.DirectConnect.prototype](#apidoc.module.vogels.AWS.DirectConnect.prototype)

#### <a name="apidoc.element.vogels.AWS.DirectConnect.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DirectConnect.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DirectConnect.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DirectoryService"></a>[module vogels.AWS.DirectoryService](#apidoc.module.vogels.AWS.DirectoryService)

#### <a name="apidoc.element.vogels.AWS.DirectoryService.DirectoryService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DirectoryService ()](#apidoc.element.vogels.AWS.DirectoryService.DirectoryService)
- description and source-code
```javascript
DirectoryService = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DirectoryService.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.</span>__super__ (config)](#apidoc.element.vogels.AWS.DirectoryService.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DirectoryService.prototype"></a>[module vogels.AWS.DirectoryService.prototype](#apidoc.module.vogels.AWS.DirectoryService.prototype)

#### <a name="apidoc.element.vogels.AWS.DirectoryService.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DirectoryService.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DirectoryService.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DynamoDB"></a>[module vogels.AWS.DynamoDB](#apidoc.module.vogels.AWS.DynamoDB)

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DynamoDB"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDB ()](#apidoc.element.vogels.AWS.DynamoDB.DynamoDB)
- description and source-code
```javascript
DynamoDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
...

'''js
Account.config({tableName: 'AccountsTable'});
'''

You can also pass in a custom instance of the aws-sdk DynamoDB client
'''js
var dynamodb = new AWS.DynamoDB();
Account.config({dynamodb: dynamodb});

// or globally use custom DynamoDB instance
// all defined models will now use this driver
vogels.dynamoDriver(dynamodb);
'''
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>DocumentClient (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient)
- description and source-code
```javascript
function DocumentClient(options) {
  var self = this;
  self.options = options || {};
  self.configure(self.options);
}
```
- example usage
```shell
...
  utils = require('./utils'),
  AWS   = require('aws-sdk');

var serializer = module.exports;

var internals = {};

internals.docClient = new AWS.DynamoDB.DocumentClient();

internals.createSet = function(value) {
if(_.isArray(value) ) {
  return internals.docClient.createSet(value);
} else {
  return internals.docClient.createSet([value]);
}
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.</span>__super__ (config)](#apidoc.element.vogels.AWS.DynamoDB.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DynamoDB.DocumentClient.prototype"></a>[module vogels.AWS.DynamoDB.DocumentClient.prototype](#apidoc.module.vogels.AWS.DynamoDB.DocumentClient.prototype)

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.batchGet"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>batchGet (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.batchGet)
- description and source-code
```javascript
batchGet = function (params, callback) {
  var self = this;
  var request = self.service.batchGetItem(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.batchWrite"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>batchWrite (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.batchWrite)
- description and source-code
```javascript
batchWrite = function (params, callback) {
  var self = this;
  var request = self.service.batchWriteItem(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.bindServiceObject"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>bindServiceObject (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.bindServiceObject)
- description and source-code
```javascript
function bindServiceObject(options) {
  var self = this;
  options = options || {};

  if (!self.service) {
    self.service = new AWS.DynamoDB(options);
  } else {
    var config = AWS.util.copy(self.service.config);
    self.service = new self.service.constructor.__super__(config);
    self.service.config.params =
      AWS.util.merge(self.service.config.params || {}, options.params);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.configure"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>configure (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.configure)
- description and source-code
```javascript
function configure(options) {
  var self = this;
  self.service = options.service;
  self.bindServiceObject(options);
  self.attrValue =
    self.service.api.operations.putItem.input.members.Item.value.shape;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.constructor)
- description and source-code
```javascript
function DocumentClient(options) {
  var self = this;
  self.options = options || {};
  self.configure(self.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.createSet"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>createSet (list, options)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.createSet)
- description and source-code
```javascript
createSet = function (list, options) {
  options = options || {};
  return new DynamoDBSet(list, options);
}
```
- example usage
```shell
...

var internals = {};

internals.docClient = new AWS.DynamoDB.DocumentClient();

internals.createSet = function(value) {
  if(_.isArray(value) ) {
    return internals.docClient.createSet(value);
  } else {
    return internals.docClient.createSet([value]);
  }
};

var serialize = internals.serialize = {
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.delete"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>delete (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.delete)
- description and source-code
```javascript
delete = function (params, callback) {
  var self = this;
  var request = self.service.deleteItem(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.get"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>get (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.get)
- description and source-code
```javascript
get = function (params, callback) {
  var self = this;
  var request = self.service.getItem(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
...
'''

### Saving Models to DynamoDB
With your models defined, we can start saving them to DynamoDB.

'''js
Account.create({email: 'foo@example.com', name: 'Foo Bar', age: 21}, function (err, acc) {
  console.log('created account in DynamoDB', acc.get('email'));
});
'''

You can also first instantiate a model and then save it.

'''js
var acc = new Account({email: 'test@example.com', name: 'Test Example'});
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.getTranslator"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>getTranslator ()](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.getTranslator)
- description and source-code
```javascript
getTranslator = function () {
  return new Translator({attrValue: this.attrValue});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.put"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>put (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.put)
- description and source-code
```javascript
function put(params, callback) {
  var self = this;
  var request = self.service.putItem(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.query"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>query (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.query)
- description and source-code
```javascript
query = function (params, callback) {
  var self = this;
  var request = self.service.query(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
...
### Query
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.scan"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>scan (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.scan)
- description and source-code
```javascript
scan = function (params, callback) {
  var self = this;
  var request = self.service.scan(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
...

### Scan
Vogels provides a flexible and chainable api for scanning over all your items
This api is very similar to the query api.

'''js
// scan all accounts, returning the first page or results
Account.scan().exec(callback);

// scan all accounts, this time loading all results
// note this will potentially make several calls to DynamoDB
// in order to load all results
Account
.scan()
.loadAll()
...
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.setupRequest"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>setupRequest (request)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.setupRequest)
- description and source-code
```javascript
function setupRequest(request) {
  var self = this;
  var translator = self.getTranslator();
  var operation = request.operation;
  var inputShape = request.service.api.operations[operation].input;
  request._events.validate.unshift(function(req) {
    req.rawParams = AWS.util.copy(req.params);
    req.params = translator.translateInput(req.rawParams, inputShape);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.setupResponse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>setupResponse (request)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.setupResponse)
- description and source-code
```javascript
function setupResponse(request) {
  var self = this;
  var translator = self.getTranslator();
  var outputShape = self.service.api.operations[request.operation].output;
  request.on('extractData', function(response) {
    response.data = translator.translateOutput(response.data, outputShape);
  });

  var response = request.response;
  response.nextPage = function(cb) {
    var resp = this;
    var req = resp.request;
    var config;
    var service = req.service;
    var operation = req.operation;
    try {
      config = service.paginationConfig(operation, true);
    } catch (e) { resp.error = e; }

    if (!resp.hasNextPage()) {
      if (cb) cb(resp.error, null);
      else if (resp.error) throw resp.error;
      return null;
    }

    var params = AWS.util.copy(req.rawParams);
    if (!resp.nextPageTokens) {
      return cb ? cb(null, null) : null;
    } else {
      var inputTokens = config.inputToken;
      if (typeof inputTokens === 'string') inputTokens = [inputTokens];
      for (var i = 0; i < inputTokens.length; i++) {
        params[inputTokens[i]] = resp.nextPageTokens[i];
      }
      return self[operation](params, cb);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.update"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.DocumentClient.prototype.</span>update (params, callback)](#apidoc.element.vogels.AWS.DynamoDB.DocumentClient.prototype.update)
- description and source-code
```javascript
update = function (params, callback) {
  var self = this;
  var request = self.service.updateItem(params);
  self.setupRequest(request);
  self.setupResponse(request);
  if (typeof callback === 'function') {
    request.send(callback);
  }
  return request;
}
```
- example usage
```shell
...
vogels.AWS.config.loadFromPath('credentials.json');
'''

When running on EC2 its recommended to leverage EC2 IAM roles. If you have configured your instance to use IAM roles, Vogels will
 automatically select these credentials for use in your application, and you do not need to manually provide credentials in any
other format.

'''js
var vogels = require('vogels');
vogels.AWS.config.update({region: "REGION"}); // region must be set
'''

You can also directly pass in your access key id, secret and region.
  * Its recommend you not hard-code credentials inside an application. Use this method only for small personal scripts or for testing
 purposes.

'''js
var vogels = require('vogels');
...
```



# <a name="apidoc.module.vogels.AWS.DynamoDB.prototype"></a>[module vogels.AWS.DynamoDB.prototype](#apidoc.module.vogels.AWS.DynamoDB.prototype)

#### <a name="apidoc.element.vogels.AWS.DynamoDB.prototype.checkCrc32"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>checkCrc32 (resp)](#apidoc.element.vogels.AWS.DynamoDB.prototype.checkCrc32)
- description and source-code
```javascript
function checkCrc32(resp) {
  if (!resp.httpResponse.streaming && !resp.request.service.crc32IsValid(resp)) {
    resp.error = AWS.util.error(new Error(), {
      code: 'CRC32CheckFailed',
      message: 'CRC32 integrity check failed',
      retryable: true
    });
    resp.request.haltHandlersOnError();
    throw (resp.error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DynamoDB.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.prototype.crc32IsValid"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>crc32IsValid (resp)](#apidoc.element.vogels.AWS.DynamoDB.prototype.crc32IsValid)
- description and source-code
```javascript
function crc32IsValid(resp) {
  var crc = resp.httpResponse.headers['x-amz-crc32'];
  if (!crc) return true; // no (valid) CRC32 header
  return parseInt(crc, 10) === AWS.util.crypto.crc32(resp.httpResponse.body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.prototype.retryDelays"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>retryDelays (retryCount)](#apidoc.element.vogels.AWS.DynamoDB.prototype.retryDelays)
- description and source-code
```javascript
function retryDelays(retryCount) {
  var delay = retryCount > 0 ? (50 * Math.pow(2, retryCount - 1)) : 0;
  return delay;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDB.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDB.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.DynamoDB.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  if (request.service.config.dynamoDbCrc32) {
    request.removeListener('extractData', AWS.EventListeners.Json.EXTRACT_DATA);
    request.addListener('extractData', this.checkCrc32);
    request.addListener('extractData', AWS.EventListeners.Json.EXTRACT_DATA);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DynamoDBStreams"></a>[module vogels.AWS.DynamoDBStreams](#apidoc.module.vogels.AWS.DynamoDBStreams)

#### <a name="apidoc.element.vogels.AWS.DynamoDBStreams.DynamoDBStreams"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>DynamoDBStreams ()](#apidoc.element.vogels.AWS.DynamoDBStreams.DynamoDBStreams)
- description and source-code
```javascript
DynamoDBStreams = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.DynamoDBStreams.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.</span>__super__ (config)](#apidoc.element.vogels.AWS.DynamoDBStreams.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.DynamoDBStreams.prototype"></a>[module vogels.AWS.DynamoDBStreams.prototype](#apidoc.module.vogels.AWS.DynamoDBStreams.prototype)

#### <a name="apidoc.element.vogels.AWS.DynamoDBStreams.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.DynamoDBStreams.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.DynamoDBStreams.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EC2"></a>[module vogels.AWS.EC2](#apidoc.module.vogels.AWS.EC2)

#### <a name="apidoc.element.vogels.AWS.EC2.EC2"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2 ()](#apidoc.element.vogels.AWS.EC2.EC2)
- description and source-code
```javascript
EC2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2.</span>__super__ (config)](#apidoc.element.vogels.AWS.EC2.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EC2.prototype"></a>[module vogels.AWS.EC2.prototype](#apidoc.module.vogels.AWS.EC2.prototype)

#### <a name="apidoc.element.vogels.AWS.EC2.prototype.buildCopySnapshotPresignedUrl"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>buildCopySnapshotPresignedUrl (req, done)](#apidoc.element.vogels.AWS.EC2.prototype.buildCopySnapshotPresignedUrl)
- description and source-code
```javascript
function buildCopySnapshotPresignedUrl(req, done) {
  if (req.params.PresignedUrl || req._subRequest) {
    return done();
  }

  req.params = AWS.util.copy(req.params);
  req.params.DestinationRegion = req.service.config.region;

  var config = AWS.util.copy(req.service.config);
  delete config.endpoint;
  config.region = req.params.SourceRegion;
  var svc = new req.service.constructor(config);
  var newReq = svc[req.operation](req.params);
  newReq._subRequest = true;
  newReq.presign(function(err, url) {
    if (err) done(err);
    else {
      req.params.PresignedUrl = url;
      done();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.EC2.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2.prototype.extractError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>extractError (resp)](#apidoc.element.vogels.AWS.EC2.prototype.extractError)
- description and source-code
```javascript
function extractError(resp) {
  // EC2 nests the error code and message deeper than other AWS Query services.
  var httpResponse = resp.httpResponse;
  var data = new AWS.XML.Parser().parse(httpResponse.body.toString() || '');
  if (data.Errors) {
    resp.error = AWS.util.error(new Error(), {
      code: data.Errors.Error.Code,
      message: data.Errors.Error.Message
    });
  } else {
    resp.error = AWS.util.error(new Error(), {
      code: httpResponse.statusCode,
      message: null
    });
  }
  resp.error.requestId = data.RequestID || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.EC2.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.removeListener('extractError', AWS.EventListeners.Query.EXTRACT_ERROR);
  request.addListener('extractError', this.extractError);

  if (request.operation === 'copySnapshot') {
    request.onAsync('validate', this.buildCopySnapshotPresignedUrl);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EC2MetadataCredentials"></a>[module vogels.AWS.EC2MetadataCredentials](#apidoc.module.vogels.AWS.EC2MetadataCredentials)

#### <a name="apidoc.element.vogels.AWS.EC2MetadataCredentials.EC2MetadataCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EC2MetadataCredentials (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials.EC2MetadataCredentials)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2MetadataCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.EC2MetadataCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EC2MetadataCredentials.prototype"></a>[module vogels.AWS.EC2MetadataCredentials.prototype](#apidoc.module.vogels.AWS.EC2MetadataCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.EC2MetadataCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.EC2MetadataCredentials.prototype.constructor)
- description and source-code
```javascript
function EC2MetadataCredentials(options) {
  AWS.Credentials.call(this);

  options = options ? AWS.util.copy(options) : {};
  if (!options.httpOptions) options.httpOptions = {};
  options.httpOptions = AWS.util.merge(
    {timeout: this.defaultTimeout}, options.httpOptions);

  this.metadataService = new AWS.MetadataService(options);
  this.metadata = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EC2MetadataCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EC2MetadataCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.EC2MetadataCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  if (!callback) callback = function(err) { if (err) throw err; };

  self.metadataService.loadCredentials(function (err, creds) {
    if (!err) {
      self.expired = false;
      self.metadata = creds;
      self.accessKeyId = creds.AccessKeyId;
      self.secretAccessKey = creds.SecretAccessKey;
      self.sessionToken = creds.Token;
      self.expireTime = new Date(creds.Expiration);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ECR"></a>[module vogels.AWS.ECR](#apidoc.module.vogels.AWS.ECR)

#### <a name="apidoc.element.vogels.AWS.ECR.ECR"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ECR ()](#apidoc.element.vogels.AWS.ECR.ECR)
- description and source-code
```javascript
ECR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ECR.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ECR.</span>__super__ (config)](#apidoc.element.vogels.AWS.ECR.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ECR.prototype"></a>[module vogels.AWS.ECR.prototype](#apidoc.module.vogels.AWS.ECR.prototype)

#### <a name="apidoc.element.vogels.AWS.ECR.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ECR.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ECR.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ECS"></a>[module vogels.AWS.ECS](#apidoc.module.vogels.AWS.ECS)

#### <a name="apidoc.element.vogels.AWS.ECS.ECS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ECS ()](#apidoc.element.vogels.AWS.ECS.ECS)
- description and source-code
```javascript
ECS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ECS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ECS.</span>__super__ (config)](#apidoc.element.vogels.AWS.ECS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ECS.prototype"></a>[module vogels.AWS.ECS.prototype](#apidoc.module.vogels.AWS.ECS.prototype)

#### <a name="apidoc.element.vogels.AWS.ECS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ECS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ECS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EFS"></a>[module vogels.AWS.EFS](#apidoc.module.vogels.AWS.EFS)

#### <a name="apidoc.element.vogels.AWS.EFS.EFS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EFS ()](#apidoc.element.vogels.AWS.EFS.EFS)
- description and source-code
```javascript
EFS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EFS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EFS.</span>__super__ (config)](#apidoc.element.vogels.AWS.EFS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EFS.prototype"></a>[module vogels.AWS.EFS.prototype](#apidoc.module.vogels.AWS.EFS.prototype)

#### <a name="apidoc.element.vogels.AWS.EFS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EFS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.EFS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ELB"></a>[module vogels.AWS.ELB](#apidoc.module.vogels.AWS.ELB)

#### <a name="apidoc.element.vogels.AWS.ELB.ELB"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ELB ()](#apidoc.element.vogels.AWS.ELB.ELB)
- description and source-code
```javascript
ELB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ELB.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ELB.</span>__super__ (config)](#apidoc.element.vogels.AWS.ELB.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ELB.prototype"></a>[module vogels.AWS.ELB.prototype](#apidoc.module.vogels.AWS.ELB.prototype)

#### <a name="apidoc.element.vogels.AWS.ELB.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ELB.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ELB.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EMR"></a>[module vogels.AWS.EMR](#apidoc.module.vogels.AWS.EMR)

#### <a name="apidoc.element.vogels.AWS.EMR.EMR"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EMR ()](#apidoc.element.vogels.AWS.EMR.EMR)
- description and source-code
```javascript
EMR = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EMR.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EMR.</span>__super__ (config)](#apidoc.element.vogels.AWS.EMR.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EMR.prototype"></a>[module vogels.AWS.EMR.prototype](#apidoc.module.vogels.AWS.EMR.prototype)

#### <a name="apidoc.element.vogels.AWS.EMR.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EMR.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.EMR.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ES"></a>[module vogels.AWS.ES](#apidoc.module.vogels.AWS.ES)

#### <a name="apidoc.element.vogels.AWS.ES.ES"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ES ()](#apidoc.element.vogels.AWS.ES.ES)
- description and source-code
```javascript
ES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ES.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ES.</span>__super__ (config)](#apidoc.element.vogels.AWS.ES.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ES.prototype"></a>[module vogels.AWS.ES.prototype](#apidoc.module.vogels.AWS.ES.prototype)

#### <a name="apidoc.element.vogels.AWS.ES.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ES.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ES.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ElastiCache"></a>[module vogels.AWS.ElastiCache](#apidoc.module.vogels.AWS.ElastiCache)

#### <a name="apidoc.element.vogels.AWS.ElastiCache.ElastiCache"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ElastiCache ()](#apidoc.element.vogels.AWS.ElastiCache.ElastiCache)
- description and source-code
```javascript
ElastiCache = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElastiCache.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.</span>__super__ (config)](#apidoc.element.vogels.AWS.ElastiCache.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ElastiCache.prototype"></a>[module vogels.AWS.ElastiCache.prototype](#apidoc.module.vogels.AWS.ElastiCache.prototype)

#### <a name="apidoc.element.vogels.AWS.ElastiCache.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ElastiCache.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ElastiCache.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ElasticBeanstalk"></a>[module vogels.AWS.ElasticBeanstalk](#apidoc.module.vogels.AWS.ElasticBeanstalk)

#### <a name="apidoc.element.vogels.AWS.ElasticBeanstalk.ElasticBeanstalk"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticBeanstalk ()](#apidoc.element.vogels.AWS.ElasticBeanstalk.ElasticBeanstalk)
- description and source-code
```javascript
ElasticBeanstalk = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElasticBeanstalk.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.</span>__super__ (config)](#apidoc.element.vogels.AWS.ElasticBeanstalk.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ElasticBeanstalk.prototype"></a>[module vogels.AWS.ElasticBeanstalk.prototype](#apidoc.module.vogels.AWS.ElasticBeanstalk.prototype)

#### <a name="apidoc.element.vogels.AWS.ElasticBeanstalk.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ElasticBeanstalk.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ElasticBeanstalk.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ElasticTranscoder"></a>[module vogels.AWS.ElasticTranscoder](#apidoc.module.vogels.AWS.ElasticTranscoder)

#### <a name="apidoc.element.vogels.AWS.ElasticTranscoder.ElasticTranscoder"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ElasticTranscoder ()](#apidoc.element.vogels.AWS.ElasticTranscoder.ElasticTranscoder)
- description and source-code
```javascript
ElasticTranscoder = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ElasticTranscoder.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.</span>__super__ (config)](#apidoc.element.vogels.AWS.ElasticTranscoder.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ElasticTranscoder.prototype"></a>[module vogels.AWS.ElasticTranscoder.prototype](#apidoc.module.vogels.AWS.ElasticTranscoder.prototype)

#### <a name="apidoc.element.vogels.AWS.ElasticTranscoder.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ElasticTranscoder.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ElasticTranscoder.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Endpoint"></a>[module vogels.AWS.Endpoint](#apidoc.module.vogels.AWS.Endpoint)

#### <a name="apidoc.element.vogels.AWS.Endpoint.Endpoint"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Endpoint (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint.Endpoint)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Endpoint.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Endpoint.</span>__super__ ()](#apidoc.element.vogels.AWS.Endpoint.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Endpoint.prototype"></a>[module vogels.AWS.Endpoint.prototype](#apidoc.module.vogels.AWS.Endpoint.prototype)

#### <a name="apidoc.element.vogels.AWS.Endpoint.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Endpoint.prototype.</span>constructor (endpoint, config)](#apidoc.element.vogels.AWS.Endpoint.prototype.constructor)
- description and source-code
```javascript
function Endpoint(endpoint, config) {
  AWS.util.hideProperties(this, ['slashes', 'auth', 'hash', 'search', 'query']);

  if (typeof endpoint === 'undefined' || endpoint === null) {
    throw new Error('Invalid endpoint: ' + endpoint);
  } else if (typeof endpoint !== 'string') {
    return AWS.util.copy(endpoint);
  }

  if (!endpoint.match(/^http/)) {
    var useSSL = config && config.sslEnabled !== undefined ?
      config.sslEnabled : AWS.config.sslEnabled;
    endpoint = (useSSL ? 'https' : 'http') + '://' + endpoint;
  }

  AWS.util.update(this, AWS.util.urlParse(endpoint));

  // Ensure the port property is set as an integer
  if (this.port) {
    this.port = parseInt(this.port, 10);
  } else {
    this.port = this.protocol === 'https:' ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EnvironmentCredentials"></a>[module vogels.AWS.EnvironmentCredentials](#apidoc.module.vogels.AWS.EnvironmentCredentials)

#### <a name="apidoc.element.vogels.AWS.EnvironmentCredentials.EnvironmentCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>EnvironmentCredentials (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials.EnvironmentCredentials)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EnvironmentCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EnvironmentCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.EnvironmentCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.EnvironmentCredentials.prototype"></a>[module vogels.AWS.EnvironmentCredentials.prototype](#apidoc.module.vogels.AWS.EnvironmentCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.EnvironmentCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EnvironmentCredentials.prototype.</span>constructor (envPrefix)](#apidoc.element.vogels.AWS.EnvironmentCredentials.prototype.constructor)
- description and source-code
```javascript
function EnvironmentCredentials(envPrefix) {
  AWS.Credentials.call(this);
  this.envPrefix = envPrefix;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.EnvironmentCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.EnvironmentCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.EnvironmentCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  if (!callback) callback = function(err) { if (err) throw err; };

  if (process === undefined) {
    callback(new Error('No process info available'));
    return;
  }

  var keys = ['ACCESS_KEY_ID', 'SECRET_ACCESS_KEY', 'SESSION_TOKEN'];
  var values = [];

  for (var i = 0; i < keys.length; i++) {
    var prefix = '';
    if (this.envPrefix) prefix = this.envPrefix + '_';
    values[i] = process.env[prefix + keys[i]];
    if (!values[i] && keys[i] !== 'SESSION_TOKEN') {
      callback(new Error('Variable ' + prefix + keys[i] + ' not set.'));
      return;
    }
  }

  this.expired = false;
  AWS.Credentials.apply(this, values);
  callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.FileSystemCredentials"></a>[module vogels.AWS.FileSystemCredentials](#apidoc.module.vogels.AWS.FileSystemCredentials)

#### <a name="apidoc.element.vogels.AWS.FileSystemCredentials.FileSystemCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>FileSystemCredentials (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials.FileSystemCredentials)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.FileSystemCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.FileSystemCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.FileSystemCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.FileSystemCredentials.prototype"></a>[module vogels.AWS.FileSystemCredentials.prototype](#apidoc.module.vogels.AWS.FileSystemCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.FileSystemCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.FileSystemCredentials.prototype.</span>constructor (filename)](#apidoc.element.vogels.AWS.FileSystemCredentials.prototype.constructor)
- description and source-code
```javascript
function FileSystemCredentials(filename) {
  AWS.Credentials.call(this);
  this.filename = filename;
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.FileSystemCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.FileSystemCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.FileSystemCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  if (!callback) callback = function(err) { if (err) throw err; };
  try {
    var creds = JSON.parse(AWS.util.readFileSync(this.filename));
    AWS.Credentials.call(this, creds);
    if (!this.accessKeyId || !this.secretAccessKey) {
      throw new Error('Credentials not set in ' + this.filename);
    }
    this.expired = false;
    callback();
  } catch (err) {
    callback(err);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Firehose"></a>[module vogels.AWS.Firehose](#apidoc.module.vogels.AWS.Firehose)

#### <a name="apidoc.element.vogels.AWS.Firehose.Firehose"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Firehose ()](#apidoc.element.vogels.AWS.Firehose.Firehose)
- description and source-code
```javascript
Firehose = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Firehose.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Firehose.</span>__super__ (config)](#apidoc.element.vogels.AWS.Firehose.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Firehose.prototype"></a>[module vogels.AWS.Firehose.prototype](#apidoc.module.vogels.AWS.Firehose.prototype)

#### <a name="apidoc.element.vogels.AWS.Firehose.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Firehose.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Firehose.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.GameLift"></a>[module vogels.AWS.GameLift](#apidoc.module.vogels.AWS.GameLift)

#### <a name="apidoc.element.vogels.AWS.GameLift.GameLift"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>GameLift ()](#apidoc.element.vogels.AWS.GameLift.GameLift)
- description and source-code
```javascript
GameLift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.GameLift.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.GameLift.</span>__super__ (config)](#apidoc.element.vogels.AWS.GameLift.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.GameLift.prototype"></a>[module vogels.AWS.GameLift.prototype](#apidoc.module.vogels.AWS.GameLift.prototype)

#### <a name="apidoc.element.vogels.AWS.GameLift.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.GameLift.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.GameLift.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Glacier"></a>[module vogels.AWS.Glacier](#apidoc.module.vogels.AWS.Glacier)

#### <a name="apidoc.element.vogels.AWS.Glacier.Glacier"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Glacier ()](#apidoc.element.vogels.AWS.Glacier.Glacier)
- description and source-code
```javascript
Glacier = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.</span>__super__ (config)](#apidoc.element.vogels.AWS.Glacier.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Glacier.prototype"></a>[module vogels.AWS.Glacier.prototype](#apidoc.module.vogels.AWS.Glacier.prototype)

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.addGlacierApiVersion"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>addGlacierApiVersion (request)](#apidoc.element.vogels.AWS.Glacier.prototype.addGlacierApiVersion)
- description and source-code
```javascript
function addGlacierApiVersion(request) {
  var version = request.service.api.apiVersion;
  request.httpRequest.headers['x-amz-glacier-version'] = version;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.addTreeHashHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>addTreeHashHeaders (request)](#apidoc.element.vogels.AWS.Glacier.prototype.addTreeHashHeaders)
- description and source-code
```javascript
function addTreeHashHeaders(request) {
  if (request.params.body === undefined) return;

  var hashes = request.service.computeChecksums(request.params.body);
  request.httpRequest.headers['X-Amz-Content-Sha256'] = hashes.linearHash;

  if (!request.httpRequest.headers['x-amz-sha256-tree-hash']) {
    request.httpRequest.headers['x-amz-sha256-tree-hash'] = hashes.treeHash;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.buildHashTree"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>buildHashTree (hashes)](#apidoc.element.vogels.AWS.Glacier.prototype.buildHashTree)
- description and source-code
```javascript
function buildHashTree(hashes) {
  // merge leaf nodes
  while (hashes.length > 1) {
    var tmpHashes = [];
    for (var i = 0; i < hashes.length; i += 2) {
      if (hashes[i + 1]) {
        var tmpHash = new AWS.util.Buffer(64);
        tmpHash.write(hashes[i], 0, 32, 'binary');
        tmpHash.write(hashes[i + 1], 32, 32, 'binary');
        tmpHashes.push(AWS.util.crypto.sha256(tmpHash));
      } else {
        tmpHashes.push(hashes[i]);
      }
    }
    hashes = tmpHashes;
  }

  return AWS.util.crypto.toHex(hashes[0]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.computeChecksums"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>computeChecksums (data)](#apidoc.element.vogels.AWS.Glacier.prototype.computeChecksums)
- description and source-code
```javascript
function computeChecksums(data) {
  if (!AWS.util.Buffer.isBuffer(data)) data = new AWS.util.Buffer(data);

  var mb = 1024 * 1024;
  var hashes = [];
  var hash = AWS.util.crypto.createHash('sha256');

  // build leaf nodes in 1mb chunks
  for (var i = 0; i < data.length; i += mb) {
    var chunk = data.slice(i, Math.min(i + mb, data.length));
    hash.update(chunk);
    hashes.push(AWS.util.crypto.sha256(chunk));
  }

  return {
    linearHash: hash.digest('hex'),
    treeHash: this.buildHashTree(hashes)
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Glacier.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.Glacier.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  if (Array.isArray(request._events.validate)) {
    request._events.validate.unshift(this.validateAccountId);
  } else {
    request.on('validate', this.validateAccountId);
  }
  request.removeListener('afterBuild',
    AWS.EventListeners.Core.COMPUTE_SHA256);
  request.on('build', this.addGlacierApiVersion);
  request.on('build', this.addTreeHashHeaders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Glacier.prototype.validateAccountId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Glacier.prototype.</span>validateAccountId (request)](#apidoc.element.vogels.AWS.Glacier.prototype.validateAccountId)
- description and source-code
```javascript
function validateAccountId(request) {
  if (request.params.accountId !== undefined) return;
  request.params = AWS.util.copy(request.params);
  request.params.accountId = '-';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.HttpClient"></a>[module vogels.AWS.HttpClient](#apidoc.module.vogels.AWS.HttpClient)

#### <a name="apidoc.element.vogels.AWS.HttpClient.HttpClient"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpClient ()](#apidoc.element.vogels.AWS.HttpClient.HttpClient)
- description and source-code
```javascript
HttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.</span>__super__ ()](#apidoc.element.vogels.AWS.HttpClient.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient.getInstance"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.</span>getInstance ()](#apidoc.element.vogels.AWS.HttpClient.getInstance)
- description and source-code
```javascript
function getInstance() {
  if (this.singleton === undefined) {
    this.singleton = new this();
  }
  return this.singleton;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.HttpClient.prototype"></a>[module vogels.AWS.HttpClient.prototype](#apidoc.module.vogels.AWS.HttpClient.prototype)

#### <a name="apidoc.element.vogels.AWS.HttpClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.HttpClient.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient.prototype.handleRequest"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>handleRequest (httpRequest, httpOptions, callback, errCallback)](#apidoc.element.vogels.AWS.HttpClient.prototype.handleRequest)
- description and source-code
```javascript
function handleRequest(httpRequest, httpOptions, callback, errCallback) {
  var self = this;
  var cbAlreadyCalled = false;
  var endpoint = httpRequest.endpoint;
  var pathPrefix = '';
  if (!httpOptions) httpOptions = {};
  if (httpOptions.proxy) {
    pathPrefix = endpoint.protocol + '//' + endpoint.hostname;
    if (endpoint.port !== 80 && endpoint.port !== 443) {
      pathPrefix += ':' + endpoint.port;
    }
    endpoint = new AWS.Endpoint(httpOptions.proxy);
  }

  var useSSL = endpoint.protocol === 'https:';
  var http = useSSL ? require('https') : require('http');
  var options = {
    host: endpoint.hostname,
    port: endpoint.port,
    method: httpRequest.method,
    headers: httpRequest.headers,
    path: pathPrefix + httpRequest.path
  };

  if (useSSL && !httpOptions.agent) {
    options.agent = this.sslAgent();
  }

  AWS.util.update(options, httpOptions);
  delete options.proxy; // proxy isn't an HTTP option
  delete options.timeout; // timeout isn't an HTTP option

  var stream = http.request(options, function (httpResp) {
    if (cbAlreadyCalled) return; cbAlreadyCalled = true;

    callback(httpResp);
    httpResp.emit('headers', httpResp.statusCode, httpResp.headers);
  });
  httpRequest.stream = stream; // attach stream to httpRequest

  // timeout support
  stream.setTimeout(httpOptions.timeout || 0, function() {
    if (cbAlreadyCalled) return; cbAlreadyCalled = true;

    var msg = 'Connection timed out after ' + httpOptions.timeout + 'ms';
    errCallback(AWS.util.error(new Error(msg), {code: 'TimeoutError'}));
    stream.abort();
  });

  stream.on('error', function() {
    if (cbAlreadyCalled) return; cbAlreadyCalled = true;
    errCallback.apply(this, arguments);
  });

  var expect = httpRequest.headers.Expect || httpRequest.headers.expect;
  if (expect === '100-continue') {
    stream.on('continue', function() {
      self.writeBody(stream, httpRequest);
    });
  } else {
    this.writeBody(stream, httpRequest);
  }

  return stream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient.prototype.progressStream"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>progressStream (stream, httpRequest)](#apidoc.element.vogels.AWS.HttpClient.prototype.progressStream)
- description and source-code
```javascript
function progressStream(stream, httpRequest) {
  var numBytes = 0;
  var totalBytes = httpRequest.headers['Content-Length'];
  var writer = new WritableStream();
  writer._write = function(chunk, encoding, callback) {
    if (chunk) {
      numBytes += chunk.length;
      stream.emit('sendProgress', {
        loaded: numBytes, total: totalBytes
      });
    }
    callback();
  };
  return writer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient.prototype.sslAgent"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>sslAgent ()](#apidoc.element.vogels.AWS.HttpClient.prototype.sslAgent)
- description and source-code
```javascript
function sslAgent() {
  var https = require('https');

  if (!AWS.NodeHttpClient.sslAgent) {
    AWS.NodeHttpClient.sslAgent = new https.Agent({rejectUnauthorized: true});
    AWS.NodeHttpClient.sslAgent.setMaxListeners(0);

    // delegate maxSockets to globalAgent
    Object.defineProperty(AWS.NodeHttpClient.sslAgent, 'maxSockets', {
      enumerable: true,
      get: function() { return https.globalAgent.maxSockets; }
    });
  }
  return AWS.NodeHttpClient.sslAgent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpClient.prototype.writeBody"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpClient.prototype.</span>writeBody (stream, httpRequest)](#apidoc.element.vogels.AWS.HttpClient.prototype.writeBody)
- description and source-code
```javascript
function writeBody(stream, httpRequest) {
  var body = httpRequest.body;

  if (body && WritableStream && ReadableStream) { // progress support
    if (!(body instanceof Stream)) body = AWS.util.buffer.toStream(body);
    body.pipe(this.progressStream(stream, httpRequest));
  }

  if (body instanceof Stream) {
    body.pipe(stream);
  } else if (body) {
    stream.end(body);
  } else {
    stream.end();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.HttpRequest"></a>[module vogels.AWS.HttpRequest](#apidoc.module.vogels.AWS.HttpRequest)

#### <a name="apidoc.element.vogels.AWS.HttpRequest.HttpRequest"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpRequest (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest.HttpRequest)
- description and source-code
```javascript
function HttpRequest(endpoint, region, customUserAgent) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent(customUserAgent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpRequest.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.</span>__super__ ()](#apidoc.element.vogels.AWS.HttpRequest.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.HttpRequest.prototype"></a>[module vogels.AWS.HttpRequest.prototype](#apidoc.module.vogels.AWS.HttpRequest.prototype)

#### <a name="apidoc.element.vogels.AWS.HttpRequest.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>constructor (endpoint, region, customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest.prototype.constructor)
- description and source-code
```javascript
function HttpRequest(endpoint, region, customUserAgent) {
  endpoint = new AWS.Endpoint(endpoint);
  this.method = 'POST';
  this.path = endpoint.path || '/';
  this.headers = {};
  this.body = '';
  this.endpoint = endpoint;
  this.region = region;
  this.setUserAgent(customUserAgent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpRequest.prototype.pathname"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>pathname ()](#apidoc.element.vogels.AWS.HttpRequest.prototype.pathname)
- description and source-code
```javascript
function pathname() {
  return this.path.split('?', 1)[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpRequest.prototype.search"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>search ()](#apidoc.element.vogels.AWS.HttpRequest.prototype.search)
- description and source-code
```javascript
function search() {
  var query = this.path.split('?', 2)[1];
  if (query) {
    query = AWS.util.queryStringParse(query);
    return AWS.util.queryParamsToString(query);
  }
  return '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpRequest.prototype.setUserAgent"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpRequest.prototype.</span>setUserAgent (customUserAgent)](#apidoc.element.vogels.AWS.HttpRequest.prototype.setUserAgent)
- description and source-code
```javascript
function setUserAgent(customUserAgent) {
  var prefix = AWS.util.isBrowser() ? 'X-Amz-' : '';
  var customSuffix = '';
  if (typeof customUserAgent === 'string' && customUserAgent) {
    customSuffix += ' ' + customUserAgent;
  }
  this.headers[prefix + 'User-Agent'] = AWS.util.userAgent() + customSuffix;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.HttpResponse"></a>[module vogels.AWS.HttpResponse](#apidoc.module.vogels.AWS.HttpResponse)

#### <a name="apidoc.element.vogels.AWS.HttpResponse.HttpResponse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>HttpResponse ()](#apidoc.element.vogels.AWS.HttpResponse.HttpResponse)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpResponse.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpResponse.</span>__super__ ()](#apidoc.element.vogels.AWS.HttpResponse.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.HttpResponse.prototype"></a>[module vogels.AWS.HttpResponse.prototype](#apidoc.module.vogels.AWS.HttpResponse.prototype)

#### <a name="apidoc.element.vogels.AWS.HttpResponse.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpResponse.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.HttpResponse.prototype.constructor)
- description and source-code
```javascript
function HttpResponse() {
  this.statusCode = undefined;
  this.headers = {};
  this.body = undefined;
  this.streaming = false;
  this.stream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.HttpResponse.prototype.createUnbufferedStream"></a>[function <span class="apidocSignatureSpan">vogels.AWS.HttpResponse.prototype.</span>createUnbufferedStream ()](#apidoc.element.vogels.AWS.HttpResponse.prototype.createUnbufferedStream)
- description and source-code
```javascript
function createUnbufferedStream() {
  this.streaming = true;
  return this.stream;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.IAM"></a>[module vogels.AWS.IAM](#apidoc.module.vogels.AWS.IAM)

#### <a name="apidoc.element.vogels.AWS.IAM.IAM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>IAM ()](#apidoc.element.vogels.AWS.IAM.IAM)
- description and source-code
```javascript
IAM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IAM.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IAM.</span>__super__ (config)](#apidoc.element.vogels.AWS.IAM.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.IAM.prototype"></a>[module vogels.AWS.IAM.prototype](#apidoc.module.vogels.AWS.IAM.prototype)

#### <a name="apidoc.element.vogels.AWS.IAM.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IAM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.IAM.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ImportExport"></a>[module vogels.AWS.ImportExport](#apidoc.module.vogels.AWS.ImportExport)

#### <a name="apidoc.element.vogels.AWS.ImportExport.ImportExport"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ImportExport ()](#apidoc.element.vogels.AWS.ImportExport.ImportExport)
- description and source-code
```javascript
ImportExport = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ImportExport.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ImportExport.</span>__super__ (config)](#apidoc.element.vogels.AWS.ImportExport.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ImportExport.prototype"></a>[module vogels.AWS.ImportExport.prototype](#apidoc.module.vogels.AWS.ImportExport.prototype)

#### <a name="apidoc.element.vogels.AWS.ImportExport.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ImportExport.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.ImportExport.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Inspector"></a>[module vogels.AWS.Inspector](#apidoc.module.vogels.AWS.Inspector)

#### <a name="apidoc.element.vogels.AWS.Inspector.Inspector"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Inspector ()](#apidoc.element.vogels.AWS.Inspector.Inspector)
- description and source-code
```javascript
Inspector = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Inspector.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Inspector.</span>__super__ (config)](#apidoc.element.vogels.AWS.Inspector.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Inspector.prototype"></a>[module vogels.AWS.Inspector.prototype](#apidoc.module.vogels.AWS.Inspector.prototype)

#### <a name="apidoc.element.vogels.AWS.Inspector.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Inspector.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Inspector.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Iot"></a>[module vogels.AWS.Iot](#apidoc.module.vogels.AWS.Iot)

#### <a name="apidoc.element.vogels.AWS.Iot.Iot"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Iot ()](#apidoc.element.vogels.AWS.Iot.Iot)
- description and source-code
```javascript
Iot = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Iot.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Iot.</span>__super__ (config)](#apidoc.element.vogels.AWS.Iot.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Iot.prototype"></a>[module vogels.AWS.Iot.prototype](#apidoc.module.vogels.AWS.Iot.prototype)

#### <a name="apidoc.element.vogels.AWS.Iot.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Iot.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Iot.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.IotData"></a>[module vogels.AWS.IotData](#apidoc.module.vogels.AWS.IotData)

#### <a name="apidoc.element.vogels.AWS.IotData.IotData"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>IotData ()](#apidoc.element.vogels.AWS.IotData.IotData)
- description and source-code
```javascript
IotData = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IotData.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IotData.</span>__super__ (config)](#apidoc.element.vogels.AWS.IotData.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.IotData.prototype"></a>[module vogels.AWS.IotData.prototype](#apidoc.module.vogels.AWS.IotData.prototype)

#### <a name="apidoc.element.vogels.AWS.IotData.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.IotData.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IotData.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.IotData.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
    request.addListener('validateResponse', this.validateResponseBody)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IotData.prototype.validateResponseBody"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>validateResponseBody (resp)](#apidoc.element.vogels.AWS.IotData.prototype.validateResponseBody)
- description and source-code
```javascript
function validateResponseBody(resp) {
    var body = resp.httpResponse.body.toString() || '{}';
    var bodyCheck = body.trim();
    if (!bodyCheck || bodyCheck.charAt(0) !== '{') {
        resp.httpResponse.body = '';
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.IotData.prototype.validateService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.IotData.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.IotData.prototype.validateService)
- description and source-code
```javascript
function validateService() {
    if (!this.config.endpoint || this.config.endpoint.indexOf('{') >= 0) {
        var msg = 'AWS.IotData requires an explicit ' +
            ''endpoint\' configuration option.';
        throw AWS.util.error(new Error(),
            {name: 'InvalidEndpoint', message: msg});
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.JSON"></a>[module vogels.AWS.JSON](#apidoc.module.vogels.AWS.JSON)

#### <a name="apidoc.element.vogels.AWS.JSON.Builder"></a>[function <span class="apidocSignatureSpan">vogels.AWS.JSON.</span>Builder ()](#apidoc.element.vogels.AWS.JSON.Builder)
- description and source-code
```javascript
function JsonBuilder() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.JSON.Parser"></a>[function <span class="apidocSignatureSpan">vogels.AWS.JSON.</span>Parser ()](#apidoc.element.vogels.AWS.JSON.Parser)
- description and source-code
```javascript
function JsonParser() { }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.JSON.Builder.prototype"></a>[module vogels.AWS.JSON.Builder.prototype](#apidoc.module.vogels.AWS.JSON.Builder.prototype)

#### <a name="apidoc.element.vogels.AWS.JSON.Builder.prototype.build"></a>[function <span class="apidocSignatureSpan">vogels.AWS.JSON.Builder.prototype.</span>build (value, shape)](#apidoc.element.vogels.AWS.JSON.Builder.prototype.build)
- description and source-code
```javascript
build = function (value, shape) {
  return JSON.stringify(translate(value, shape));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.JSON.Parser.prototype"></a>[module vogels.AWS.JSON.Parser.prototype](#apidoc.module.vogels.AWS.JSON.Parser.prototype)

#### <a name="apidoc.element.vogels.AWS.JSON.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.JSON.Parser.prototype.</span>parse (value, shape)](#apidoc.element.vogels.AWS.JSON.Parser.prototype.parse)
- description and source-code
```javascript
parse = function (value, shape) {
  return translate(JSON.parse(value), shape);
}
```
- example usage
```shell
...
  });
};

internals.updateExpressions = function (schema, data, options) {
  var exp = expressions.serializeUpdateExpression(schema, data);

  if(options.UpdateExpression) {
    var parsed = expressions.parse(options.UpdateExpression);

    exp.expressions = _.reduce(parsed, function (result, val, key) {
if(!_.isEmpty(val)) {
  result[key] = result[key].concat(val);
}

return result;
...
```



# <a name="apidoc.module.vogels.AWS.KMS"></a>[module vogels.AWS.KMS](#apidoc.module.vogels.AWS.KMS)

#### <a name="apidoc.element.vogels.AWS.KMS.KMS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>KMS ()](#apidoc.element.vogels.AWS.KMS.KMS)
- description and source-code
```javascript
KMS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.KMS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.KMS.</span>__super__ (config)](#apidoc.element.vogels.AWS.KMS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.KMS.prototype"></a>[module vogels.AWS.KMS.prototype](#apidoc.module.vogels.AWS.KMS.prototype)

#### <a name="apidoc.element.vogels.AWS.KMS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.KMS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.KMS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Kinesis"></a>[module vogels.AWS.Kinesis](#apidoc.module.vogels.AWS.Kinesis)

#### <a name="apidoc.element.vogels.AWS.Kinesis.Kinesis"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Kinesis ()](#apidoc.element.vogels.AWS.Kinesis.Kinesis)
- description and source-code
```javascript
Kinesis = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Kinesis.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Kinesis.</span>__super__ (config)](#apidoc.element.vogels.AWS.Kinesis.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Kinesis.prototype"></a>[module vogels.AWS.Kinesis.prototype](#apidoc.module.vogels.AWS.Kinesis.prototype)

#### <a name="apidoc.element.vogels.AWS.Kinesis.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Kinesis.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Kinesis.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Lambda"></a>[module vogels.AWS.Lambda](#apidoc.module.vogels.AWS.Lambda)

#### <a name="apidoc.element.vogels.AWS.Lambda.Lambda"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Lambda ()](#apidoc.element.vogels.AWS.Lambda.Lambda)
- description and source-code
```javascript
Lambda = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Lambda.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Lambda.</span>__super__ (config)](#apidoc.element.vogels.AWS.Lambda.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Lambda.prototype"></a>[module vogels.AWS.Lambda.prototype](#apidoc.module.vogels.AWS.Lambda.prototype)

#### <a name="apidoc.element.vogels.AWS.Lambda.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Lambda.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Lambda.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MachineLearning"></a>[module vogels.AWS.MachineLearning](#apidoc.module.vogels.AWS.MachineLearning)

#### <a name="apidoc.element.vogels.AWS.MachineLearning.MachineLearning"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MachineLearning ()](#apidoc.element.vogels.AWS.MachineLearning.MachineLearning)
- description and source-code
```javascript
MachineLearning = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MachineLearning.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.</span>__super__ (config)](#apidoc.element.vogels.AWS.MachineLearning.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MachineLearning.prototype"></a>[module vogels.AWS.MachineLearning.prototype](#apidoc.module.vogels.AWS.MachineLearning.prototype)

#### <a name="apidoc.element.vogels.AWS.MachineLearning.prototype.buildEndpoint"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.prototype.</span>buildEndpoint (request)](#apidoc.element.vogels.AWS.MachineLearning.prototype.buildEndpoint)
- description and source-code
```javascript
function buildEndpoint(request) {
  var url = request.params.PredictEndpoint;
  if (url) {
    request.httpRequest.endpoint = new AWS.Endpoint(url);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MachineLearning.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MachineLearning.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MachineLearning.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MachineLearning.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.MachineLearning.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  if (request.operation === 'predict') {
    request.addListener('build', this.buildEndpoint);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MarketplaceCommerceAnalytics"></a>[module vogels.AWS.MarketplaceCommerceAnalytics](#apidoc.module.vogels.AWS.MarketplaceCommerceAnalytics)

#### <a name="apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.MarketplaceCommerceAnalytics"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceCommerceAnalytics ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.MarketplaceCommerceAnalytics)
- description and source-code
```javascript
MarketplaceCommerceAnalytics = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.</span>__super__ (config)](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MarketplaceCommerceAnalytics.prototype"></a>[module vogels.AWS.MarketplaceCommerceAnalytics.prototype](#apidoc.module.vogels.AWS.MarketplaceCommerceAnalytics.prototype)

#### <a name="apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceCommerceAnalytics.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MarketplaceCommerceAnalytics.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MarketplaceMetering"></a>[module vogels.AWS.MarketplaceMetering](#apidoc.module.vogels.AWS.MarketplaceMetering)

#### <a name="apidoc.element.vogels.AWS.MarketplaceMetering.MarketplaceMetering"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MarketplaceMetering ()](#apidoc.element.vogels.AWS.MarketplaceMetering.MarketplaceMetering)
- description and source-code
```javascript
MarketplaceMetering = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MarketplaceMetering.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.</span>__super__ (config)](#apidoc.element.vogels.AWS.MarketplaceMetering.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MarketplaceMetering.prototype"></a>[module vogels.AWS.MarketplaceMetering.prototype](#apidoc.module.vogels.AWS.MarketplaceMetering.prototype)

#### <a name="apidoc.element.vogels.AWS.MarketplaceMetering.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MarketplaceMetering.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MarketplaceMetering.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MetadataService"></a>[module vogels.AWS.MetadataService](#apidoc.module.vogels.AWS.MetadataService)

#### <a name="apidoc.element.vogels.AWS.MetadataService.MetadataService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MetadataService (options)](#apidoc.element.vogels.AWS.MetadataService.MetadataService)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MetadataService.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.</span>__super__ ()](#apidoc.element.vogels.AWS.MetadataService.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MetadataService.prototype"></a>[module vogels.AWS.MetadataService.prototype](#apidoc.module.vogels.AWS.MetadataService.prototype)

#### <a name="apidoc.element.vogels.AWS.MetadataService.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.MetadataService.prototype.constructor)
- description and source-code
```javascript
function MetadataService(options) {
  AWS.util.update(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MetadataService.prototype.loadCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>loadCredentials (callback)](#apidoc.element.vogels.AWS.MetadataService.prototype.loadCredentials)
- description and source-code
```javascript
function loadCredentials(callback) {
  var self = this;
  var basePath = '/latest/meta-data/iam/security-credentials/';
  self.loadCredentialsCallbacks.push(callback);
  if (self.loadCredentialsCallbacks.length > 1) { return; }

  function callbacks(err, creds) {
    var cb;
    while ((cb = self.loadCredentialsCallbacks.shift()) !== undefined) {
      cb(err, creds);
    }
  }

  self.request(basePath, function (err, roleName) {
    if (err) callbacks(err);
    else {
      roleName = roleName.split('\n')[0]; // grab first (and only) role
      self.request(basePath + roleName, function (credErr, credData) {
        if (credErr) callbacks(credErr);
        else {
          try {
            var credentials = JSON.parse(credData);
            callbacks(null, credentials);
          } catch (parseError) {
            callbacks(parseError);
          }
        }
      });
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MetadataService.prototype.request"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MetadataService.prototype.</span>request (path, callback)](#apidoc.element.vogels.AWS.MetadataService.prototype.request)
- description and source-code
```javascript
function request(path, callback) {
  path = path || '/';

  var data = '';
  var http = AWS.HttpClient.getInstance();
  var httpRequest = new AWS.HttpRequest('http://' + this.host + path);
  httpRequest.method = 'GET';
  var httpOptions = this.httpOptions;

  process.nextTick(function() {
    http.handleRequest(httpRequest, httpOptions, function(httpResponse) {
      httpResponse.on('data', function(chunk) { data += chunk.toString(); });
      httpResponse.on('end', function() { callback(null, data); });
    }, callback);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MobileAnalytics"></a>[module vogels.AWS.MobileAnalytics](#apidoc.module.vogels.AWS.MobileAnalytics)

#### <a name="apidoc.element.vogels.AWS.MobileAnalytics.MobileAnalytics"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>MobileAnalytics ()](#apidoc.element.vogels.AWS.MobileAnalytics.MobileAnalytics)
- description and source-code
```javascript
MobileAnalytics = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.MobileAnalytics.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.</span>__super__ (config)](#apidoc.element.vogels.AWS.MobileAnalytics.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.MobileAnalytics.prototype"></a>[module vogels.AWS.MobileAnalytics.prototype](#apidoc.module.vogels.AWS.MobileAnalytics.prototype)

#### <a name="apidoc.element.vogels.AWS.MobileAnalytics.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.MobileAnalytics.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.MobileAnalytics.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Model"></a>[module vogels.AWS.Model](#apidoc.module.vogels.AWS.Model)

#### <a name="apidoc.element.vogels.AWS.Model.Api"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Api (api, options)](#apidoc.element.vogels.AWS.Model.Api)
- description and source-code
```javascript
function Api(api, options) {
  api = api || {};
  options = options || {};
  options.api = this;

  api.metadata = api.metadata || {};

  property(this, 'isApi', true, false);
  property(this, 'apiVersion', api.metadata.apiVersion);
  property(this, 'endpointPrefix', api.metadata.endpointPrefix);
  property(this, 'signingName', api.metadata.signingName);
  property(this, 'globalEndpoint', api.metadata.globalEndpoint);
  property(this, 'signatureVersion', api.metadata.signatureVersion);
  property(this, 'jsonVersion', api.metadata.jsonVersion);
  property(this, 'targetPrefix', api.metadata.targetPrefix);
  property(this, 'protocol', api.metadata.protocol);
  property(this, 'timestampFormat', api.metadata.timestampFormat);
  property(this, 'xmlNamespaceUri', api.metadata.xmlNamespace);
  property(this, 'abbreviation', api.metadata.serviceAbbreviation);
  property(this, 'fullName', api.metadata.serviceFullName);

  memoizedProperty(this, 'className', function() {
    var name = api.metadata.serviceAbbreviation || api.metadata.serviceFullName;
    if (!name) return null;

    name = name.replace(/^Amazon|AWS\s*|\(.*|\s+|\W+/g, '');
    if (name === 'ElasticLoadBalancing') name = 'ELB';
    return name;
  });

  property(this, 'operations', new Collection(api.operations, options, function(name, operation) {
    return new Operation(name, operation, options);
  }, util.string.lowerFirst));

  property(this, 'shapes', new Collection(api.shapes, options, function(name, shape) {
    return Shape.create(shape, options);
  }));

  property(this, 'paginators', new Collection(api.paginators, options, function(name, paginator) {
    return new Paginator(name, paginator, options);
  }));

  property(this, 'waiters', new Collection(api.waiters, options, function(name, waiter) {
    return new ResourceWaiter(name, waiter, options);
  }, util.string.lowerFirst));

  if (options.documentation) {
    property(this, 'documentation', api.documentation);
    property(this, 'documentationUrl', api.documentationUrl);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Model.Operation"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Operation (name, operation, options)](#apidoc.element.vogels.AWS.Model.Operation)
- description and source-code
```javascript
function Operation(name, operation, options) {
  options = options || {};

  property(this, 'name', operation.name || name);
  property(this, 'api', options.api, false);

  operation.http = operation.http || {};
  property(this, 'httpMethod', operation.http.method || 'POST');
  property(this, 'httpPath', operation.http.requestUri || '/');

  memoizedProperty(this, 'input', function() {
    if (!operation.input) {
      return new Shape.create({type: 'structure'}, options);
    }
    return Shape.create(operation.input, options);
  });

  memoizedProperty(this, 'output', function() {
    if (!operation.output) {
      return new Shape.create({type: 'structure'}, options);
    }
    return Shape.create(operation.output, options);
  });

  memoizedProperty(this, 'errors', function() {
    var list = [];
    if (!operation.errors) return null;

    for (var i = 0; i < operation.errors.length; i++) {
      list.push(Shape.create(operation.errors[i], options));
    }

    return list;
  });

  memoizedProperty(this, 'paginator', function() {
    return options.api.paginators[name];
  });

  if (options.documentation) {
    property(this, 'documentation', operation.documentation);
    property(this, 'documentationUrl', operation.documentationUrl);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Model.Paginator"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Paginator (name, paginator)](#apidoc.element.vogels.AWS.Model.Paginator)
- description and source-code
```javascript
function Paginator(name, paginator) {
  property(this, 'inputToken', paginator.input_token);
  property(this, 'limitKey', paginator.limit_key);
  property(this, 'moreResults', paginator.more_results);
  property(this, 'outputToken', paginator.output_token);
  property(this, 'resultKey', paginator.result_key);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Model.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>ResourceWaiter (name, waiter, options)](#apidoc.element.vogels.AWS.Model.ResourceWaiter)
- description and source-code
```javascript
function ResourceWaiter(name, waiter, options) {
  options = options || {};

  function InnerResourceWaiter() {
    property(this, 'name', name);
    property(this, 'api', options.api, false);

    if (waiter.operation) {
      property(this, 'operation', util.string.lowerFirst(waiter.operation));
    }

    var self = this, map = {
      ignoreErrors: 'ignore_errors',
      successType: 'success_type',
      successValue: 'success_value',
      successPath: 'success_path',
      acceptorType: 'acceptor_type',
      acceptorValue: 'acceptor_value',
      acceptorPath: 'acceptor_path',
      failureType: 'failure_type',
      failureValue: 'failure_value',
      failurePath: 'success_path',
      interval: 'interval',
      maxAttempts: 'max_attempts'
    };
    Object.keys(map).forEach(function(key) {
      var value = waiter[map[key]];
      if (value) property(self, key, value);
    });
  }

  if (options.api) {
    var proto = null;
    if (waiter['extends']) {
      proto = options.api.waiters[waiter['extends']];
    } else if (name !== '__default__') {
      proto = options.api.waiters['__default__'];
    }

    if (proto) InnerResourceWaiter.prototype = proto;
  }

  return new InnerResourceWaiter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Model.Shape"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Model.</span>Shape (shape, options, memberName)](#apidoc.element.vogels.AWS.Model.Shape)
- description and source-code
```javascript
function Shape(shape, options, memberName) {
  options = options || {};

  property(this, 'shape', shape.shape);
  property(this, 'api', options.api, false);
  property(this, 'type', shape.type);
  property(this, 'enum', shape.enum);
  property(this, 'min', shape.min);
  property(this, 'max', shape.max);
  property(this, 'pattern', shape.pattern);
  property(this, 'location', shape.location || this.location || 'body');
  property(this, 'name', this.name || shape.xmlName || shape.queryName ||
    shape.locationName || memberName);
  property(this, 'isStreaming', shape.streaming || this.isStreaming || false);
  property(this, 'isComposite', shape.isComposite || false);
  property(this, 'isShape', true, false);
  property(this, 'isQueryName', shape.queryName ? true : false, false);
  property(this, 'isLocationName', shape.locationName ? true : false, false);

  if (options.documentation) {
    property(this, 'documentation', shape.documentation);
    property(this, 'documentationUrl', shape.documentationUrl);
  }

  if (shape.xmlAttribute) {
    property(this, 'isXmlAttribute', shape.xmlAttribute || false);
  }

  // type conversion and parsing
  property(this, 'defaultValue', null);
  this.toWireFormat = function(value) {
    if (value === null || value === undefined) return '';
    return value;
  };
  this.toType = function(value) { return value; };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.NodeHttpClient"></a>[module vogels.AWS.NodeHttpClient](#apidoc.module.vogels.AWS.NodeHttpClient)

#### <a name="apidoc.element.vogels.AWS.NodeHttpClient.NodeHttpClient"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>NodeHttpClient ()](#apidoc.element.vogels.AWS.NodeHttpClient.NodeHttpClient)
- description and source-code
```javascript
NodeHttpClient = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.NodeHttpClient.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.NodeHttpClient.</span>__super__ ()](#apidoc.element.vogels.AWS.NodeHttpClient.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.OpsWorks"></a>[module vogels.AWS.OpsWorks](#apidoc.module.vogels.AWS.OpsWorks)

#### <a name="apidoc.element.vogels.AWS.OpsWorks.OpsWorks"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>OpsWorks ()](#apidoc.element.vogels.AWS.OpsWorks.OpsWorks)
- description and source-code
```javascript
OpsWorks = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.OpsWorks.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.</span>__super__ (config)](#apidoc.element.vogels.AWS.OpsWorks.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.OpsWorks.prototype"></a>[module vogels.AWS.OpsWorks.prototype](#apidoc.module.vogels.AWS.OpsWorks.prototype)

#### <a name="apidoc.element.vogels.AWS.OpsWorks.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.OpsWorks.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.OpsWorks.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ParamValidator"></a>[module vogels.AWS.ParamValidator](#apidoc.module.vogels.AWS.ParamValidator)

#### <a name="apidoc.element.vogels.AWS.ParamValidator.ParamValidator"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ParamValidator (validation)](#apidoc.element.vogels.AWS.ParamValidator.ParamValidator)
- description and source-code
```javascript
function ParamValidator(validation) {
  if (validation === true || validation === undefined) {
    validation = {'min': true};
  }
  this.validation = validation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.</span>__super__ ()](#apidoc.element.vogels.AWS.ParamValidator.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ParamValidator.prototype"></a>[module vogels.AWS.ParamValidator.prototype](#apidoc.module.vogels.AWS.ParamValidator.prototype)

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>constructor (validation)](#apidoc.element.vogels.AWS.ParamValidator.prototype.constructor)
- description and source-code
```javascript
function ParamValidator(validation) {
  if (validation === true || validation === undefined) {
    validation = {'min': true};
  }
  this.validation = validation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.fail"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>fail (code, message)](#apidoc.element.vogels.AWS.ParamValidator.prototype.fail)
- description and source-code
```javascript
function fail(code, message) {
  this.errors.push(AWS.util.error(new Error(message), {code: code}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validate"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validate (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validate)
- description and source-code
```javascript
function validate(shape, params, context) {
  this.errors = [];
  this.validateMember(shape, params || {}, context || 'params');

  if (this.errors.length > 1) {
    var msg = this.errors.join('\n* ');
    msg = 'There were ' + this.errors.length +
      ' validation errors:\n* ' + msg;
    throw AWS.util.error(new Error(msg),
      {code: 'MultipleValidationErrors', errors: this.errors});
  } else if (this.errors.length === 1) {
    throw this.errors[0];
  } else {
    return true;
  }
}
```
- example usage
```shell
...
var Schema = module.exports = function (config) {
  this.secondaryIndexes = {};
  this.globalIndexes = {};

  var context = {hashKey : config.hashKey};

  var self = this;
  Joi.validate(config, internals.configSchema, { context: context }, function (err, data) {
if(err) {
  var msg = 'Invalid table schema, check your config ';
  throw new Error(msg + err.annotate());
}

self.hashKey    = data.hashKey;
self.rangeKey   = data.rangeKey;
...
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateEnum"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateEnum (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateEnum)
- description and source-code
```javascript
function validateRange(shape, value, context) {
  if (this.validation['enum'] && shape['enum'] !== undefined) {
    // Fail if the string value is not present in the enum list
    if (shape['enum'].indexOf(value) === -1) {
      this.fail('EnumError', 'Found string value of ' + value + ', but '
        + 'expected ' + shape['enum'].join('|') + ' for ' + context);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateList"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateList (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateList)
- description and source-code
```javascript
function validateList(shape, params, context) {
  if (this.validateType(params, context, [Array])) {
    this.validateRange(shape, params.length, context, 'list member count');
    // validate array members
    for (var i = 0; i < params.length; i++) {
      this.validateMember(shape.member, params[i], context + '[' + i + ']');
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateMap"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateMap (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateMap)
- description and source-code
```javascript
function validateMap(shape, params, context) {
  if (this.validateType(params, context, ['object'], 'map')) {
    // Build up a count of map members to validate range traits.
    var mapCount = 0;
    for (var param in params) {
      if (!params.hasOwnProperty(param)) continue;
      // Validate any map key trait constraints
      this.validateMember(shape.key, param,
                          context + '[key=\'' + param + '\']')
      this.validateMember(shape.value, params[param],
                          context + '[\'' + param + '\']');
      mapCount++;
    }
    this.validateRange(shape, mapCount, context, 'map member count');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateMember"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateMember (shape, param, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateMember)
- description and source-code
```javascript
function validateMember(shape, param, context) {
  switch (shape.type) {
    case 'structure':
      return this.validateStructure(shape, param, context);
    case 'list':
      return this.validateList(shape, param, context);
    case 'map':
      return this.validateMap(shape, param, context);
    default:
      return this.validateScalar(shape, param, context);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateNumber"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateNumber (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateNumber)
- description and source-code
```javascript
function validateNumber(shape, value, context) {
  if (value === null || value === undefined) return;
  if (typeof value === 'string') {
    var castedValue = parseFloat(value);
    if (castedValue.toString() === value) value = castedValue;
  }
  if (this.validateType(value, context, ['number'])) {
    this.validateRange(shape, value, context, 'numeric value');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validatePattern"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validatePattern (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validatePattern)
- description and source-code
```javascript
function validatePattern(shape, value, context) {
  if (this.validation['pattern'] && shape['pattern'] !== undefined) {
    if (!(new RegExp(shape['pattern'])).test(value)) {
      this.fail('PatternMatchError', 'Provided value "' + value + '" '
        + 'does not match regex pattern /' + shape['pattern'] + '/ for '
        + context);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validatePayload"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validatePayload (value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validatePayload)
- description and source-code
```javascript
function validatePayload(value, context) {
  if (value === null || value === undefined) return;
  if (typeof value === 'string') return;
  if (value && typeof value.byteLength === 'number') return; // typed arrays
  if (AWS.util.isNode()) { // special check for buffer/stream in Node.js
    var Stream = AWS.util.nodeRequire('stream').Stream;
    if (AWS.util.Buffer.isBuffer(value) || value instanceof Stream) return;
  }

  var types = ['Buffer', 'Stream', 'File', 'Blob', 'ArrayBuffer', 'DataView'];
  if (value) {
    for (var i = 0; i < types.length; i++) {
      if (AWS.util.isType(value, types[i])) return;
      if (AWS.util.typeName(value.constructor) === types[i]) return;
    }
  }

  this.fail('InvalidParameterType', 'Expected ' + context + ' to be a ' +
    'string, Buffer, Stream, Blob, or typed array object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateRange"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateRange (shape, value, context, descriptor)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateRange)
- description and source-code
```javascript
function validateRange(shape, value, context, descriptor) {
  if (this.validation['min']) {
    if (shape['min'] !== undefined && value < shape['min']) {
      this.fail('MinRangeError', 'Expected ' + descriptor + ' >= '
        + shape['min'] + ', but found ' + value + ' for ' + context);
    }
  }
  if (this.validation['max']) {
    if (shape['max'] !== undefined && value > shape['max']) {
      this.fail('MaxRangeError', 'Expected ' + descriptor + ' <= '
        + shape['max'] + ', but found ' + value + ' for ' + context);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateScalar"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateScalar (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateScalar)
- description and source-code
```javascript
function validateScalar(shape, value, context) {
  switch (shape.type) {
    case null:
    case undefined:
    case 'string':
      return this.validateString(shape, value, context);
    case 'base64':
    case 'binary':
      return this.validatePayload(value, context);
    case 'integer':
    case 'float':
      return this.validateNumber(shape, value, context);
    case 'boolean':
      return this.validateType(value, context, ['boolean']);
    case 'timestamp':
      return this.validateType(value, context, [Date,
        /^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}(\.\d+)?Z$/, 'number'],
        'Date object, ISO-8601 string, or a UNIX timestamp');
    default:
      return this.fail('UnkownType', 'Unhandled type ' +
                       shape.type + ' for ' + context);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateString"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateString (shape, value, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateString)
- description and source-code
```javascript
function validateString(shape, value, context) {
  if (this.validateType(value, context, ['string'])) {
    this.validateEnum(shape, value, context);
    this.validateRange(shape, value.length, context, 'string length');
    this.validatePattern(shape, value, context);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateStructure"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateStructure (shape, params, context)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateStructure)
- description and source-code
```javascript
function validateStructure(shape, params, context) {
  this.validateType(params, context, ['object'], 'structure');

  var paramName;
  for (var i = 0; shape.required && i < shape.required.length; i++) {
    paramName = shape.required[i];
    var value = params[paramName];
    if (value === undefined || value === null) {
      this.fail('MissingRequiredParameter',
        'Missing required key \'' + paramName + '\' in ' + context);
    }
  }

  // validate hash members
  for (paramName in params) {
    if (!params.hasOwnProperty(paramName)) continue;

    var paramValue = params[paramName],
        memberShape = shape.members[paramName];

    if (memberShape !== undefined) {
      var memberContext = [context, paramName].join('.');
      this.validateMember(memberShape, paramValue, memberContext);
    } else {
      this.fail('UnexpectedParameter',
        'Unexpected key \'' + paramName + '\' found in ' + context);
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ParamValidator.prototype.validateType"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ParamValidator.prototype.</span>validateType (value, context, acceptedTypes, type)](#apidoc.element.vogels.AWS.ParamValidator.prototype.validateType)
- description and source-code
```javascript
function validateType(value, context, acceptedTypes, type) {
  // We will not log an error for null or undefined, but we will return
  // false so that callers know that the expected type was not strictly met.
  if (value === null || value === undefined) return false;

  var foundInvalidType = false;
  for (var i = 0; i < acceptedTypes.length; i++) {
    if (typeof acceptedTypes[i] === 'string') {
      if (typeof value === acceptedTypes[i]) return true;
    } else if (acceptedTypes[i] instanceof RegExp) {
      if ((value || '').toString().match(acceptedTypes[i])) return true;
    } else {
      if (value instanceof acceptedTypes[i]) return true;
      if (AWS.util.isType(value, acceptedTypes[i])) return true;
      if (!type && !foundInvalidType) acceptedTypes = acceptedTypes.slice();
      acceptedTypes[i] = AWS.util.typeName(acceptedTypes[i]);
    }
    foundInvalidType = true;
  }

  var acceptedType = type;
  if (!acceptedType) {
    acceptedType = acceptedTypes.join(', ').replace(/,([^,]+)$/, ', or$1');
  }

  var vowel = acceptedType.match(/^[aeiou]/i) ? 'n' : '';
  this.fail('InvalidParameterType', 'Expected ' + context + ' to be a' +
            vowel + ' ' + acceptedType);
  return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.RDS"></a>[module vogels.AWS.RDS](#apidoc.module.vogels.AWS.RDS)

#### <a name="apidoc.element.vogels.AWS.RDS.RDS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>RDS ()](#apidoc.element.vogels.AWS.RDS.RDS)
- description and source-code
```javascript
RDS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.RDS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.RDS.</span>__super__ (config)](#apidoc.element.vogels.AWS.RDS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.RDS.prototype"></a>[module vogels.AWS.RDS.prototype](#apidoc.module.vogels.AWS.RDS.prototype)

#### <a name="apidoc.element.vogels.AWS.RDS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.RDS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.RDS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Redshift"></a>[module vogels.AWS.Redshift](#apidoc.module.vogels.AWS.Redshift)

#### <a name="apidoc.element.vogels.AWS.Redshift.Redshift"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Redshift ()](#apidoc.element.vogels.AWS.Redshift.Redshift)
- description and source-code
```javascript
Redshift = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Redshift.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Redshift.</span>__super__ (config)](#apidoc.element.vogels.AWS.Redshift.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Redshift.prototype"></a>[module vogels.AWS.Redshift.prototype](#apidoc.module.vogels.AWS.Redshift.prototype)

#### <a name="apidoc.element.vogels.AWS.Redshift.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Redshift.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Redshift.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Request"></a>[module vogels.AWS.Request](#apidoc.module.vogels.AWS.Request)

#### <a name="apidoc.element.vogels.AWS.Request.Request"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Request (service, operation, params)](#apidoc.element.vogels.AWS.Request.Request)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;
  var customUserAgent = service.config.customUserAgent;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region, customUserAgent);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');
  this._haltHandlersOnError = false;

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.</span>__super__ ()](#apidoc.element.vogels.AWS.Request.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Request.prototype"></a>[module vogels.AWS.Request.prototype](#apidoc.module.vogels.AWS.Request.prototype)

#### <a name="apidoc.element.vogels.AWS.Request.prototype.abort"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>abort ()](#apidoc.element.vogels.AWS.Request.prototype.abort)
- description and source-code
```javascript
function abort() {
  this.removeAllListeners('validateResponse');
  this.removeAllListeners('extractError');
  this.on('validateResponse', function addAbortedError(resp) {
    resp.error = AWS.util.error(new Error('Request aborted by user'), {
       code: 'RequestAbortedError', retryable: false
    });
  });

  if (this.httpRequest.stream) { // abort HTTP stream
    this.httpRequest.stream.abort();
    if (this.httpRequest._abortCallback) {
       this.httpRequest._abortCallback();
    } else {
      this.removeAllListeners('send'); // haven't sent yet, so let's not
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.addListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addListener (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.addListener)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.addListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addListeners (listeners)](#apidoc.element.vogels.AWS.Request.prototype.addListeners)
- description and source-code
```javascript
function addListeners(listeners) {
  var self = this;

  // extract listeners if parameter is an SequentialExecutor object
  if (listeners._events) listeners = listeners._events;

  AWS.util.each(listeners, function(event, callbacks) {
    if (typeof callbacks === 'function') callbacks = [callbacks];
    AWS.util.arrayEach(callbacks, function(callback) {
      self.on(event, callback);
    });
  });

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.addNamedAsyncListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.vogels.AWS.Request.prototype.addNamedAsyncListener)
- description and source-code
```javascript
function addNamedAsyncListener(name, eventName, callback) {
  callback._isAsync = true;
  return this.addNamedListener(name, eventName, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.addNamedListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.vogels.AWS.Request.prototype.addNamedListener)
- description and source-code
```javascript
function addNamedListener(name, eventName, callback) {
  this[name] = callback;
  this.addListener(eventName, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.addNamedListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>addNamedListeners (callback)](#apidoc.element.vogels.AWS.Request.prototype.addNamedListeners)
- description and source-code
```javascript
function addNamedListeners(callback) {
  var self = this;
  callback(
    function() {
      self.addNamedListener.apply(self, arguments);
    },
    function() {
      self.addNamedAsyncListener.apply(self, arguments);
    }
  );
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.build"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>build (callback)](#apidoc.element.vogels.AWS.Request.prototype.build)
- description and source-code
```javascript
function build(callback) {
  return this.runTo('send', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.buildAsGet"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>buildAsGet (request)](#apidoc.element.vogels.AWS.Request.prototype.buildAsGet)
- description and source-code
```javascript
function buildAsGet(request) {
  request.httpRequest.method = 'GET';
  request.httpRequest.path = request.service.endpoint.path +
                             '?' + request.httpRequest.body;
  request.httpRequest.body = '';

  // don't need these headers on a GET request
  delete request.httpRequest.headers['Content-Length'];
  delete request.httpRequest.headers['Content-Type'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.callListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>callListeners (listeners, args, doneCallback, prevError)](#apidoc.element.vogels.AWS.Request.prototype.callListeners)
- description and source-code
```javascript
function callListeners(listeners, args, doneCallback, prevError) {
  var self = this;
  var error = prevError || null;

  function callNextListener(err) {
    if (err) {
      error = AWS.util.error(error || new Error(), err);
      if (self._haltHandlersOnError) {
        return doneCallback.call(self, error);
      }
    }
    self.callListeners(listeners, args, doneCallback, error);
  }

  while (listeners.length > 0) {
    var listener = listeners.shift();
    if (listener._isAsync) { // asynchronous listener
      listener.apply(self, args.concat([callNextListener]));
      return; // stop here, callNextListener will continue
    } else { // synchronous listener
      try {
        listener.apply(self, args);
      } catch (err) {
        error = AWS.util.error(error || new Error(), err);
      }
      if (error && self._haltHandlersOnError) {
        doneCallback.call(self, error);
        return;
      }
    }
  }
  doneCallback.call(self, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>constructor (service, operation, params)](#apidoc.element.vogels.AWS.Request.prototype.constructor)
- description and source-code
```javascript
function Request(service, operation, params) {
  var endpoint = service.endpoint;
  var region = service.config.region;
  var customUserAgent = service.config.customUserAgent;

  // global endpoints sign as us-east-1
  if (service.isGlobalEndpoint) region = 'us-east-1';

  this.domain = domain && domain.active;
  this.service = service;
  this.operation = operation;
  this.params = params || {};
  this.httpRequest = new AWS.HttpRequest(endpoint, region, customUserAgent);
  this.startTime = AWS.util.date.getDate();

  this.response = new AWS.Response(this);
  this._asm = new AcceptorStateMachine(fsm.states, 'validate');
  this._haltHandlersOnError = false;

  AWS.SequentialExecutor.call(this);
  this.emit = this.emitEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.createReadStream"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>createReadStream ()](#apidoc.element.vogels.AWS.Request.prototype.createReadStream)
- description and source-code
```javascript
function createReadStream() {
  var streams = AWS.util.nodeRequire('stream');
  var req = this;
  var stream = null;

  if (AWS.HttpClient.streamsApiVersion === 2) {
    stream = new streams.PassThrough();
    req.send();
  } else {
    stream = new streams.Stream();
    stream.readable = true;

    stream.sent = false;
    stream.on('newListener', function(event) {
      if (!stream.sent && event === 'data') {
        stream.sent = true;
        process.nextTick(function() { req.send(); });
      }
    });
  }

  this.on('httpHeaders', function streamHeaders(statusCode, headers, resp) {
    if (statusCode < 300) {
      req.removeListener('httpData', AWS.EventListeners.Core.HTTP_DATA);
      req.removeListener('httpError', AWS.EventListeners.Core.HTTP_ERROR);
      req.on('httpError', function streamHttpError(error) {
        resp.error = error;
        resp.error.retryable = false;
      });

      var httpStream = resp.httpResponse.createUnbufferedStream();
      if (AWS.HttpClient.streamsApiVersion === 2) {
        httpStream.pipe(stream);
      } else {
        httpStream.on('data', function(arg) {
          stream.emit('data', arg);
        });
        httpStream.on('end', function() {
          stream.emit('end');
        });
      }

      httpStream.on('error', function(err) {
        stream.emit('error', err);
      });
    }
  });

  this.on('error', function(err) {
    stream.emit('error', err);
  });

  return stream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.eachItem"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>eachItem (callback)](#apidoc.element.vogels.AWS.Request.prototype.eachItem)
- description and source-code
```javascript
function eachItem(callback) {
  var self = this;
  function wrappedCallback(err, data) {
    if (err) return callback(err, null);
    if (data === null) return callback(null, null);

    var config = self.service.paginationConfig(self.operation);
    var resultKey = config.resultKey;
    if (Array.isArray(resultKey)) resultKey = resultKey[0];
    var results = AWS.util.jamespath.query(resultKey, data);
    AWS.util.arrayEach(results, function(result) {
      AWS.util.arrayEach(result, function(item) { callback(null, item); });
    });
  }

  this.eachPage(wrappedCallback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.eachPage"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>eachPage (callback)](#apidoc.element.vogels.AWS.Request.prototype.eachPage)
- description and source-code
```javascript
function eachPage(callback) {
  // Make all callbacks async-ish
  callback = AWS.util.fn.makeAsync(callback, 3);

  function wrappedCallback(response) {
    callback.call(response, response.error, response.data, function (result) {
      if (result === false) return;

      if (response.hasNextPage()) {
        response.nextPage().on('complete', wrappedCallback).send();
      } else {
        callback.call(response, null, null, AWS.util.fn.noop);
      }
    });
  }

  this.on('complete', wrappedCallback).send();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.emit"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.vogels.AWS.Request.prototype.emit)
- description and source-code
```javascript
function emit(eventName, eventArgs, doneCallback) {
  if (!doneCallback) doneCallback = function() { };
  var listeners = this.listeners(eventName);
  var count = listeners.length;
  this.callListeners(listeners, eventArgs, doneCallback);
  return count > 0;
}
```
- example usage
```shell
...
var streamMode = false;
var combinedStream = new Readable({objectMode: true});

if(!callback) {
  streamMode = true;
  callback = function (err) {
    if(err) {
      combinedStream.emit('error', err);
    }
  };
}

var scanFuncs = [];
_.times(self.totalSegments, function(segment) {
  var scn = new Scan(self.table, self.serializer);
...
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.emitEvent"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>emitEvent (eventName, args, done)](#apidoc.element.vogels.AWS.Request.prototype.emitEvent)
- description and source-code
```javascript
function emit(eventName, args, done) {
  if (typeof args === 'function') { done = args; args = null; }
  if (!done) done = function() { };
  if (!args) args = this.eventParameters(eventName, this.response);

  var origEmit = AWS.SequentialExecutor.prototype.emit;
  origEmit.call(this, eventName, args, function (err) {
    if (err) this.response.error = err;
    done.call(this, err);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.eventParameters"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>eventParameters (eventName)](#apidoc.element.vogels.AWS.Request.prototype.eventParameters)
- description and source-code
```javascript
function eventParameters(eventName) {
  switch (eventName) {
    case 'restart':
    case 'validate':
    case 'sign':
    case 'build':
    case 'afterValidate':
    case 'afterBuild':
      return [this];
    case 'error':
      return [this.response.error, this.response];
    default:
      return [this.response];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.haltHandlersOnError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>haltHandlersOnError ()](#apidoc.element.vogels.AWS.Request.prototype.haltHandlersOnError)
- description and source-code
```javascript
function haltHandlersOnError() {
  this._haltHandlersOnError = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.isPageable"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>isPageable ()](#apidoc.element.vogels.AWS.Request.prototype.isPageable)
- description and source-code
```javascript
function isPageable() {
  return this.service.paginationConfig(this.operation) ? true : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.listeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>listeners (eventName)](#apidoc.element.vogels.AWS.Request.prototype.listeners)
- description and source-code
```javascript
function listeners(eventName) {
  return this._events[eventName] ? this._events[eventName].slice(0) : [];
}
```
- example usage
```shell
...
  }

  return callback(null, item);
});
};

internals.callBeforeHooks = function (table, name, startFun, callback) {
var listeners = table._before.listeners(name);

return async.waterfall([startFun].concat(listeners), callback);
};

Table.prototype.create = function (item, options, callback) {
var self = this;
...
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.on"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>on (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.on)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
...
### Streaming api
vogels supports a basic streaming api in addition to the callback
api for 'query', 'scan', and 'parallelScan' operations.

'''js
var stream = Account.parallelScan(4).exec();

stream.on('readable', function () {
  console.log('single parallel scan response', stream.read());
});

stream.on('end', function () {
  console.log('Parallel scan of accounts finished');
});
...
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.onAsync"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>onAsync (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.onAsync)
- description and source-code
```javascript
function onAsync(eventName, listener) {
  listener._isAsync = true;
  return this.on(eventName, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.presign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>presign (expires, callback)](#apidoc.element.vogels.AWS.Request.prototype.presign)
- description and source-code
```javascript
function presign(expires, callback) {
  if (!callback && typeof expires === 'function') {
    callback = expires;
    expires = null;
  }
  return new AWS.Signers.Presign().sign(this.toGet(), expires, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>removeAllListeners (eventName)](#apidoc.element.vogels.AWS.Request.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(eventName) {
  if (eventName) {
    delete this._events[eventName];
  } else {
    this._events = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>removeListener (eventName, listener)](#apidoc.element.vogels.AWS.Request.prototype.removeListener)
- description and source-code
```javascript
function removeListener(eventName, listener) {
  var listeners = this._events[eventName];
  if (listeners) {
    var length = listeners.length;
    var position = -1;
    for (var i = 0; i < length; ++i) {
      if (listeners[i] === listener) {
        position = i;
      }
    }
    if (position > -1) {
      listeners.splice(position, 1);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.runTo"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>runTo (state, done)](#apidoc.element.vogels.AWS.Request.prototype.runTo)
- description and source-code
```javascript
function runTo(state, done) {
  this._asm.runTo(state, done, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.send"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>send (callback)](#apidoc.element.vogels.AWS.Request.prototype.send)
- description and source-code
```javascript
function send(callback) {
  if (callback) {
    this.on('complete', function (resp) {
      callback.call(resp, resp.error, resp.data);
    });
  }
  this.runTo();

  return this.response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.toGet"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>toGet ()](#apidoc.element.vogels.AWS.Request.prototype.toGet)
- description and source-code
```javascript
function toGet() {
  if (this.service.api.protocol === 'query' ||
      this.service.api.protocol === 'ec2') {
    this.removeListener('build', this.buildAsGet);
    this.addListener('build', this.buildAsGet);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Request.prototype.toUnauthenticated"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Request.prototype.</span>toUnauthenticated ()](#apidoc.element.vogels.AWS.Request.prototype.toUnauthenticated)
- description and source-code
```javascript
function toUnauthenticated() {
  this.removeListener('validate', AWS.EventListeners.Core.VALIDATE_CREDENTIALS);
  this.removeListener('sign', AWS.EventListeners.Core.SIGN);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ResourceWaiter"></a>[module vogels.AWS.ResourceWaiter](#apidoc.module.vogels.AWS.ResourceWaiter)

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.ResourceWaiter"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>ResourceWaiter (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter.ResourceWaiter)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.</span>__super__ ()](#apidoc.element.vogels.AWS.ResourceWaiter.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.ResourceWaiter.prototype"></a>[module vogels.AWS.ResourceWaiter.prototype](#apidoc.module.vogels.AWS.ResourceWaiter.prototype)

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.prototype.checkError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>checkError (resp)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.checkError)
- description and source-code
```javascript
function checkError(resp) {
  var value = this.config.successValue;
  if (typeof value === 'number') {
    return resp.httpResponse.statusCode === value;
  } else {
    return resp.error && resp.error.code === value;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.prototype.checkSuccess"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>checkSuccess (resp)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.checkSuccess)
- description and source-code
```javascript
function checkSuccess(resp) {
  if (!this.config.successPath) {
    return resp.httpResponse.statusCode < 300;
  }

  var r = AWS.util.jamespath.find(this.config.successPath, resp.data);

  if (this.config.failureValue &&
      this.config.failureValue.indexOf(r) >= 0) {
    return null; // fast fail
  }

  if (this.expectedValue) {
    return r === this.expectedValue;
  } else {
    return r ? true : false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>constructor (service, state)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.constructor)
- description and source-code
```javascript
function constructor(service, state) {
  this.service = service;
  this.state = state;

  if (typeof this.state === 'object') {
    AWS.util.each.call(this, this.state, function (key, value) {
      this.state = key;
      this.expectedValue = value;
    });
  }

  this.loadWaiterConfig(this.state);
  if (!this.expectedValue) {
    this.expectedValue = this.config.successValue;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.prototype.loadWaiterConfig"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>loadWaiterConfig (state, noException)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.loadWaiterConfig)
- description and source-code
```javascript
function loadWaiterConfig(state, noException) {
  if (!this.service.api.waiters[state]) {
    if (noException) return;
    throw new AWS.util.error(new Error(), {
      code: 'StateNotFoundError',
      message: 'State ' + state + ' not found.'
    });
  }

  this.config = this.service.api.waiters[state];
  var config = this.config;

  // inherit acceptor data
  (function () { // anonymous function to avoid max complexity count
    config.successType = config.successType || config.acceptorType;
    config.successPath = config.successPath || config.acceptorPath;
    config.successValue = config.successValue || config.acceptorValue;
    config.failureType = config.failureType || config.acceptorType;
    config.failurePath = config.failurePath || config.acceptorPath;
    config.failureValue = config.failureValue || config.acceptorValue;
  })();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.prototype.setError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>setError (resp, retryable)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.setError)
- description and source-code
```javascript
function setError(resp, retryable) {
  resp.data = null;
  resp.error = AWS.util.error(resp.error || new Error(), {
    code: 'ResourceNotReady',
    message: 'Resource is not in the state ' + this.state,
    retryable: retryable
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.ResourceWaiter.prototype.wait"></a>[function <span class="apidocSignatureSpan">vogels.AWS.ResourceWaiter.prototype.</span>wait (params, callback)](#apidoc.element.vogels.AWS.ResourceWaiter.prototype.wait)
- description and source-code
```javascript
function wait(params, callback) {
  if (typeof params === 'function') {
    callback = params; params = undefined;
  }

  var request = this.service.makeRequest(this.config.operation, params);
  var listeners = this.Listeners[this.config.successType];
  request._waiter = this;
  request.response.maxRetries = this.config.maxAttempts;
  request.addListeners(this.Listeners.retry);
  if (listeners) request.addListeners(listeners);

  if (callback) request.send(callback);
  return request;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Response"></a>[module vogels.AWS.Response](#apidoc.module.vogels.AWS.Response)

#### <a name="apidoc.element.vogels.AWS.Response.Response"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Response (request)](#apidoc.element.vogels.AWS.Response.Response)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Response.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Response.</span>__super__ ()](#apidoc.element.vogels.AWS.Response.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Response.prototype"></a>[module vogels.AWS.Response.prototype](#apidoc.module.vogels.AWS.Response.prototype)

#### <a name="apidoc.element.vogels.AWS.Response.prototype.cacheNextPageTokens"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>cacheNextPageTokens ()](#apidoc.element.vogels.AWS.Response.prototype.cacheNextPageTokens)
- description and source-code
```javascript
function cacheNextPageTokens() {
  if (this.hasOwnProperty('nextPageTokens')) return this.nextPageTokens;
  this.nextPageTokens = undefined;

  var config = this.request.service.paginationConfig(this.request.operation);
  if (!config) return this.nextPageTokens;

  this.nextPageTokens = null;
  if (config.moreResults) {
    if (!AWS.util.jamespath.find(config.moreResults, this.data)) {
      return this.nextPageTokens;
    }
  }

  var exprs = config.outputToken;
  if (typeof exprs === 'string') exprs = [exprs];
  AWS.util.arrayEach.call(this, exprs, function (expr) {
    var output = AWS.util.jamespath.find(expr, this.data);
    if (output) {
      this.nextPageTokens = this.nextPageTokens || [];
      this.nextPageTokens.push(output);
    }
  });

  return this.nextPageTokens;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Response.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>constructor (request)](#apidoc.element.vogels.AWS.Response.prototype.constructor)
- description and source-code
```javascript
function Response(request) {
  this.request = request;
  this.data = null;
  this.error = null;
  this.retryCount = 0;
  this.redirectCount = 0;
  this.httpResponse = new AWS.HttpResponse();
  if (request) {
    this.maxRetries = request.service.numRetries();
    this.maxRedirects = request.service.config.maxRedirects;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Response.prototype.hasNextPage"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>hasNextPage ()](#apidoc.element.vogels.AWS.Response.prototype.hasNextPage)
- description and source-code
```javascript
function hasNextPage() {
  this.cacheNextPageTokens();
  if (this.nextPageTokens) return true;
  if (this.nextPageTokens === undefined) return undefined;
  else return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Response.prototype.nextPage"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Response.prototype.</span>nextPage (callback)](#apidoc.element.vogels.AWS.Response.prototype.nextPage)
- description and source-code
```javascript
function nextPage(callback) {
  var config;
  var service = this.request.service;
  var operation = this.request.operation;
  try {
    config = service.paginationConfig(operation, true);
  } catch (e) { this.error = e; }

  if (!this.hasNextPage()) {
    if (callback) callback(this.error, null);
    else if (this.error) throw this.error;
    return null;
  }

  var params = AWS.util.copy(this.request.params);
  if (!this.nextPageTokens) {
    return callback ? callback(null, null) : null;
  } else {
    var inputTokens = config.inputToken;
    if (typeof inputTokens === 'string') inputTokens = [inputTokens];
    for (var i = 0; i < inputTokens.length; i++) {
      params[inputTokens[i]] = this.nextPageTokens[i];
    }
    return service.makeRequest(this.request.operation, params, callback);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Route53"></a>[module vogels.AWS.Route53](#apidoc.module.vogels.AWS.Route53)

#### <a name="apidoc.element.vogels.AWS.Route53.Route53"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53 ()](#apidoc.element.vogels.AWS.Route53.Route53)
- description and source-code
```javascript
Route53 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Route53.</span>__super__ (config)](#apidoc.element.vogels.AWS.Route53.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Route53.prototype"></a>[module vogels.AWS.Route53.prototype](#apidoc.module.vogels.AWS.Route53.prototype)

#### <a name="apidoc.element.vogels.AWS.Route53.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Route53.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Route53.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53.prototype.sanitizeUrl"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Route53.prototype.</span>sanitizeUrl (request)](#apidoc.element.vogels.AWS.Route53.prototype.sanitizeUrl)
- description and source-code
```javascript
function sanitizeUrl(request) {
  var path = request.httpRequest.path;
  request.httpRequest.path = path.replace(/\/%2F\w+%2F/, '/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Route53.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.Route53.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.on('build', this.sanitizeUrl);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Route53Domains"></a>[module vogels.AWS.Route53Domains](#apidoc.module.vogels.AWS.Route53Domains)

#### <a name="apidoc.element.vogels.AWS.Route53Domains.Route53Domains"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Route53Domains ()](#apidoc.element.vogels.AWS.Route53Domains.Route53Domains)
- description and source-code
```javascript
Route53Domains = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Route53Domains.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.</span>__super__ (config)](#apidoc.element.vogels.AWS.Route53Domains.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Route53Domains.prototype"></a>[module vogels.AWS.Route53Domains.prototype](#apidoc.module.vogels.AWS.Route53Domains.prototype)

#### <a name="apidoc.element.vogels.AWS.Route53Domains.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Route53Domains.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Route53Domains.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.S3"></a>[module vogels.AWS.S3](#apidoc.module.vogels.AWS.S3)

#### <a name="apidoc.element.vogels.AWS.S3.S3"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>S3 ()](#apidoc.element.vogels.AWS.S3.S3)
- description and source-code
```javascript
S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.</span>ManagedUpload (options)](#apidoc.element.vogels.AWS.S3.ManagedUpload)
- description and source-code
```javascript
function ManagedUpload(options) {
  var self = this;
  AWS.SequentialExecutor.call(self);
  self.body = null;
  self.sliceFn = null;
  self.callback = null;
  self.parts = {};
  self.completeInfo = [];
  self.fillQueue = function() {
    self.callback(new Error('Unsupported body payload ' + typeof self.body));
  };

  self.configure(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.</span>__super__ (config)](#apidoc.element.vogels.AWS.S3.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.S3.ManagedUpload.prototype"></a>[module vogels.AWS.S3.ManagedUpload.prototype](#apidoc.module.vogels.AWS.S3.ManagedUpload.prototype)

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.abort"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>abort ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.abort)
- description and source-code
```javascript
abort = function () {
  this.cleanup(AWS.util.error(new Error('Request aborted by user'), {
    code: 'RequestAbortedError', retryable: false
  }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addListener (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addListener)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addListeners (listeners)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addListeners)
- description and source-code
```javascript
function addListeners(listeners) {
  var self = this;

  // extract listeners if parameter is an SequentialExecutor object
  if (listeners._events) listeners = listeners._events;

  AWS.util.each(listeners, function(event, callbacks) {
    if (typeof callbacks === 'function') callbacks = [callbacks];
    AWS.util.arrayEach(callbacks, function(callback) {
      self.on(event, callback);
    });
  });

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedAsyncListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedAsyncListener)
- description and source-code
```javascript
function addNamedAsyncListener(name, eventName, callback) {
  callback._isAsync = true;
  return this.addNamedListener(name, eventName, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedListener)
- description and source-code
```javascript
function addNamedListener(name, eventName, callback) {
  this[name] = callback;
  this.addListener(eventName, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>addNamedListeners (callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.addNamedListeners)
- description and source-code
```javascript
function addNamedListeners(callback) {
  var self = this;
  callback(
    function() {
      self.addNamedListener.apply(self, arguments);
    },
    function() {
      self.addNamedAsyncListener.apply(self, arguments);
    }
  );
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.adjustTotalBytes"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>adjustTotalBytes ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.adjustTotalBytes)
- description and source-code
```javascript
function adjustTotalBytes() {
  var self = this;
  try { // try to get totalBytes
    self.totalBytes = byteLength(self.body);
  } catch (e) { }

  // try to adjust partSize if we know payload length
  if (self.totalBytes) {
    var newPartSize = Math.ceil(self.totalBytes / self.maxTotalParts);
    if (newPartSize > self.partSize) self.partSize = newPartSize;
  } else {
    self.totalBytes = undefined;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.bindServiceObject"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>bindServiceObject (params)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.bindServiceObject)
- description and source-code
```javascript
function bindServiceObject(params) {
  params = params || {};
  var self = this;

  // bind parameters to new service object
  if (!self.service) {
    self.service = new AWS.S3({params: params});
  } else {
    var config = AWS.util.copy(self.service.config);
    self.service = new self.service.constructor.__super__(config);
    self.service.config.params =
      AWS.util.merge(self.service.config.params || {}, params);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.callListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>callListeners (listeners, args, doneCallback, prevError)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.callListeners)
- description and source-code
```javascript
function callListeners(listeners, args, doneCallback, prevError) {
  var self = this;
  var error = prevError || null;

  function callNextListener(err) {
    if (err) {
      error = AWS.util.error(error || new Error(), err);
      if (self._haltHandlersOnError) {
        return doneCallback.call(self, error);
      }
    }
    self.callListeners(listeners, args, doneCallback, error);
  }

  while (listeners.length > 0) {
    var listener = listeners.shift();
    if (listener._isAsync) { // asynchronous listener
      listener.apply(self, args.concat([callNextListener]));
      return; // stop here, callNextListener will continue
    } else { // synchronous listener
      try {
        listener.apply(self, args);
      } catch (err) {
        error = AWS.util.error(error || new Error(), err);
      }
      if (error && self._haltHandlersOnError) {
        doneCallback.call(self, error);
        return;
      }
    }
  }
  doneCallback.call(self, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.cleanup"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>cleanup (err)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.cleanup)
- description and source-code
```javascript
function cleanup(err) {
  var self = this;
  if (self.failed) return;

  // clean up stream
  if (typeof self.body.removeAllListeners === 'function' &&
      typeof self.body.resume === 'function') {
    self.body.removeAllListeners('readable');
    self.body.removeAllListeners('end');
    self.body.resume();
  }

  if (self.service.config.params.UploadId && !self.leavePartsOnError) {
    self.service.abortMultipartUpload().send();
  }

  AWS.util.each(self.parts, function(partNumber, part) {
    part.removeAllListeners('complete');
    part.abort();
  });

  self.activeParts = 0;
  self.partPos = 0;
  self.numParts = 0;
  self.totalPartNumbers = 0;
  self.parts = {};
  self.failed = true;
  self.callback(err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.configure"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>configure (options)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.configure)
- description and source-code
```javascript
function configure(options) {
  options = options || {};
  this.partSize = this.minPartSize;

  if (options.queueSize) this.queueSize = options.queueSize;
  if (options.partSize) this.partSize = options.partSize;
  if (options.leavePartsOnError) this.leavePartsOnError = true;

  if (this.partSize < this.minPartSize) {
    throw new Error('partSize must be greater than ' +
                    this.minPartSize);
  }

  this.service = options.service;
  this.bindServiceObject(options.params);
  this.validateBody();
  this.adjustTotalBytes();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.constructor)
- description and source-code
```javascript
function ManagedUpload(options) {
  var self = this;
  AWS.SequentialExecutor.call(self);
  self.body = null;
  self.sliceFn = null;
  self.callback = null;
  self.parts = {};
  self.completeInfo = [];
  self.fillQueue = function() {
    self.callback(new Error('Unsupported body payload ' + typeof self.body));
  };

  self.configure(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.emit"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.emit)
- description and source-code
```javascript
function emit(eventName, eventArgs, doneCallback) {
  if (!doneCallback) doneCallback = function() { };
  var listeners = this.listeners(eventName);
  var count = listeners.length;
  this.callListeners(listeners, eventArgs, doneCallback);
  return count > 0;
}
```
- example usage
```shell
...
var streamMode = false;
var combinedStream = new Readable({objectMode: true});

if(!callback) {
  streamMode = true;
  callback = function (err) {
    if(err) {
      combinedStream.emit('error', err);
    }
  };
}

var scanFuncs = [];
_.times(self.totalSegments, function(segment) {
  var scn = new Scan(self.table, self.serializer);
...
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.fillBuffer"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>fillBuffer ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.fillBuffer)
- description and source-code
```javascript
function fillBuffer() {
  var self = this;
  var bodyLen = byteLength(self.body);

  if (bodyLen === 0) {
    self.isDoneChunking = true;
    self.numParts = 1;
    self.nextChunk(self.body);
    return;
  }

  while (self.activeParts < self.queueSize && self.partPos < bodyLen) {
    var endPos = Math.min(self.partPos + self.partSize, bodyLen);
    var buf = self.sliceFn.call(self.body, self.partPos, endPos);
    self.partPos += self.partSize;

    if (byteLength(buf) < self.partSize || self.partPos === bodyLen) {
      self.isDoneChunking = true;
      self.numParts = self.totalPartNumbers + 1;
    }
    self.nextChunk(buf);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.fillStream"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>fillStream ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.fillStream)
- description and source-code
```javascript
function fillStream() {
  var self = this;
  if (self.activeParts >= self.queueSize) return;

  var buf = self.body.read(self.partSize - self.partBufferLength) ||
            self.body.read();
  if (buf) {
    self.partBuffers.push(buf);
    self.partBufferLength += buf.length;
    self.totalChunkedBytes += buf.length;
  }

  if (self.partBufferLength >= self.partSize) {
    // if we have single buffer we avoid copyfull concat
    var pbuf = self.partBuffers.length === 1 ?
      self.partBuffers[0] : Buffer.concat(self.partBuffers);
    self.partBuffers = [];
    self.partBufferLength = 0;

    // if we have more than partSize, push the rest back on the queue
    if (pbuf.length > self.partSize) {
      var rest = pbuf.slice(self.partSize);
      self.partBuffers.push(rest);
      self.partBufferLength += rest.length;
      pbuf = pbuf.slice(0, self.partSize);
    }

    self.nextChunk(pbuf);
  }

  if (self.isDoneChunking && !self.isDoneSending) {
    // if we have single buffer we avoid copyfull concat
    pbuf = self.partBuffers.length === 1 ?
        self.partBuffers[0] : Buffer.concat(self.partBuffers);
    self.partBuffers = [];
    self.partBufferLength = 0;
    self.totalBytes = self.totalChunkedBytes;
    self.isDoneSending = true;

    if (self.numParts === 0 || pbuf.length > 0) {
      self.numParts++;
      self.nextChunk(pbuf);
    }
  }

  self.body.read(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.finishMultiPart"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>finishMultiPart ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.finishMultiPart)
- description and source-code
```javascript
function finishMultiPart() {
  var self = this;
  var completeParams = { MultipartUpload: { Parts: self.completeInfo.slice(1) } };
  self.service.completeMultipartUpload(completeParams, function(err, data) {
    if (err) return self.cleanup(err);
    else self.callback(err, data);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.finishSinglePart"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>finishSinglePart (err, data)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.finishSinglePart)
- description and source-code
```javascript
function finishSinglePart(err, data) {
  var upload = this.request._managedUpload;
  var httpReq = this.request.httpRequest;
  var endpoint = httpReq.endpoint;
  if (err) return upload.callback(err);
  data.Location =
    [endpoint.protocol, '//', endpoint.host, httpReq.path].join('');
  data.key = this.request.params.Key; // will stay undocumented
  data.Key = this.request.params.Key;
  data.Bucket = this.request.params.Bucket;
  upload.callback(err, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.listeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>listeners (eventName)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.listeners)
- description and source-code
```javascript
function listeners(eventName) {
  return this._events[eventName] ? this._events[eventName].slice(0) : [];
}
```
- example usage
```shell
...
  }

  return callback(null, item);
});
};

internals.callBeforeHooks = function (table, name, startFun, callback) {
var listeners = table._before.listeners(name);

return async.waterfall([startFun].concat(listeners), callback);
};

Table.prototype.create = function (item, options, callback) {
var self = this;
...
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.nextChunk"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>nextChunk (chunk)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.nextChunk)
- description and source-code
```javascript
function nextChunk(chunk) {
  var self = this;
  if (self.failed) return null;

  var partNumber = ++self.totalPartNumbers;
  if (self.isDoneChunking && partNumber === 1) {
    var req = self.service.putObject({Body: chunk});
    req._managedUpload = self;
    req.on('httpUploadProgress', self.progress).send(self.finishSinglePart);
    return null;
  } else if (self.service.config.params.ContentMD5) {
    var err = AWS.util.error(new Error('The Content-MD5 you specified is invalid for multi-part uploads.'), {
      code: 'InvalidDigest', retryable: false
    });

    self.cleanup(err);
    return null;
  }

  if (self.completeInfo[partNumber] && self.completeInfo[partNumber].ETag !== null) {
    return null; // Already uploaded this part.
  }

  self.activeParts++;
  if (!self.service.config.params.UploadId) {

    if (!self.multipartReq) { // create multipart
      self.multipartReq = self.service.createMultipartUpload();
      self.multipartReq.on('success', function(resp) {
        self.service.config.params.UploadId = resp.data.UploadId;
        self.multipartReq = null;
      });
      self.queueChunks(chunk, partNumber);
      self.multipartReq.on('error', function(err) {
        self.cleanup(err);
      });
      self.multipartReq.send();
    } else {
      self.queueChunks(chunk, partNumber);
    }
  } else { // multipart is created, just send
    self.uploadPart(chunk, partNumber);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.on"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>on (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.on)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
...
### Streaming api
vogels supports a basic streaming api in addition to the callback
api for 'query', 'scan', and 'parallelScan' operations.

'''js
var stream = Account.parallelScan(4).exec();

stream.on('readable', function () {
  console.log('single parallel scan response', stream.read());
});

stream.on('end', function () {
  console.log('Parallel scan of accounts finished');
});
...
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.onAsync"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>onAsync (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.onAsync)
- description and source-code
```javascript
function onAsync(eventName, listener) {
  listener._isAsync = true;
  return this.on(eventName, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.progress"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>progress (info)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.progress)
- description and source-code
```javascript
function progress(info) {
  var upload = this._managedUpload;
  if (this.operation === 'putObject') {
    info.part = 1;
    info.key = this.params.Key;
  } else {
    upload.totalUploadedBytes += info.loaded - this._lastUploadedBytes;
    this._lastUploadedBytes = info.loaded;
    info = {
      loaded: upload.totalUploadedBytes,
      total: upload.totalBytes,
      part: this.params.PartNumber,
      key: this.params.Key
    };
  }
  upload.emit('httpUploadProgress', [info]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.queueChunks"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>queueChunks (chunk, partNumber)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.queueChunks)
- description and source-code
```javascript
function queueChunks(chunk, partNumber) {
  var self = this;
  self.multipartReq.on('success', function() {
    self.uploadPart(chunk, partNumber);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>removeAllListeners (eventName)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(eventName) {
  if (eventName) {
    delete this._events[eventName];
  } else {
    this._events = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>removeListener (eventName, listener)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.removeListener)
- description and source-code
```javascript
function removeListener(eventName, listener) {
  var listeners = this._events[eventName];
  if (listeners) {
    var length = listeners.length;
    var position = -1;
    for (var i = 0; i < length; ++i) {
      if (listeners[i] === listener) {
        position = i;
      }
    }
    if (position > -1) {
      listeners.splice(position, 1);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.send"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>send (callback)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.send)
- description and source-code
```javascript
send = function (callback) {
  var self = this;
  self.failed = false;
  self.callback = callback || function(err) { if (err) throw err; };

  var runFill = true;
  if (self.sliceFn) {
    self.fillQueue = self.fillBuffer;
  } else if (AWS.util.isNode()) {
    var Stream = AWS.util.nodeRequire('stream').Stream;
    if (self.body instanceof Stream) {
      runFill = false;
      self.fillQueue = self.fillStream;
      self.partBuffers = [];
      self.body.
        on('readable', function() { self.fillQueue(); }).
        on('end', function() {
          self.isDoneChunking = true;
          self.numParts = self.totalPartNumbers;
          self.fillQueue.call(self);
        });
    }
  }

  if (runFill) self.fillQueue.call(self);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.uploadPart"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>uploadPart (chunk, partNumber)](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.uploadPart)
- description and source-code
```javascript
function uploadPart(chunk, partNumber) {
  var self = this;

  var partParams = {
    Body: chunk,
    ContentLength: AWS.util.string.byteLength(chunk),
    PartNumber: partNumber
  };

  var partInfo = {ETag: null, PartNumber: partNumber};
  self.completeInfo[partNumber] = partInfo;

  var req = self.service.uploadPart(partParams);
  self.parts[partNumber] = req;
  req._lastUploadedBytes = 0;
  req._managedUpload = self;
  req.on('httpUploadProgress', self.progress);
  req.send(function(err, data) {
    delete self.parts[partParams.PartNumber];
    self.activeParts--;

    if (!err && (!data || !data.ETag)) {
      var message = 'No access to ETag property on response.';
      if (AWS.util.isBrowser()) {
        message += ' Check CORS configuration to expose ETag header.';
      }

      err = AWS.util.error(new Error(message), {
        code: 'ETagMissing', retryable: false
      });
    }
    if (err) return self.cleanup(err);

    partInfo.ETag = data.ETag;
    self.doneParts++;
    if (self.isDoneChunking && self.doneParts === self.numParts) {
      self.finishMultiPart();
    } else {
      self.fillQueue.call(self);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.validateBody"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.ManagedUpload.prototype.</span>validateBody ()](#apidoc.element.vogels.AWS.S3.ManagedUpload.prototype.validateBody)
- description and source-code
```javascript
function validateBody() {
  var self = this;
  self.body = self.service.config.params.Body;
  if (!self.body) throw new Error('params.Body is required');
  if (typeof self.body === 'string') {
    self.body = new AWS.util.Buffer(self.body);
  }
  self.sliceFn = AWS.util.arraySliceFn(self.body);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.S3.prototype"></a>[module vogels.AWS.S3.prototype](#apidoc.module.vogels.AWS.S3.prototype)

#### <a name="apidoc.element.vogels.AWS.S3.prototype.addContentType"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>addContentType (req)](#apidoc.element.vogels.AWS.S3.prototype.addContentType)
- description and source-code
```javascript
function addContentType(req) {
  var httpRequest = req.httpRequest;
  if (httpRequest.method === 'GET' || httpRequest.method === 'HEAD') {
    // Content-Type is not set in GET/HEAD requests
    delete httpRequest.headers['Content-Type'];
    return;
  }

  if (!httpRequest.headers['Content-Type']) { // always have a Content-Type
    httpRequest.headers['Content-Type'] = 'application/octet-stream';
  }

  var contentType = httpRequest.headers['Content-Type'];
  if (AWS.util.isBrowser()) {
    if (typeof httpRequest.body === 'string' && !contentType.match(/;\s*charset=/)) {
      var charset = '; charset=UTF-8';
      httpRequest.headers['Content-Type'] += charset;
    } else {
      var replaceFn = function(_, prefix, charsetName) {
        return prefix + charsetName.toUpperCase();
      };

      httpRequest.headers['Content-Type'] =
        contentType.replace(/(;\s*charset=)(.+)$/, replaceFn);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.addExpect100Continue"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>addExpect100Continue (req)](#apidoc.element.vogels.AWS.S3.prototype.addExpect100Continue)
- description and source-code
```javascript
function addExpect100Continue(req) {
  var len = req.httpRequest.headers['Content-Length'];
  if (AWS.util.isNode() && len >= 1024 * 1024) {
    req.httpRequest.headers['Expect'] = '100-continue';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.computeContentMd5"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>computeContentMd5 (req)](#apidoc.element.vogels.AWS.S3.prototype.computeContentMd5)
- description and source-code
```javascript
function computeContentMd5(req) {
  if (req.service.willComputeChecksums(req)) {
    var md5 = AWS.util.crypto.md5(req.httpRequest.body, 'base64');
    req.httpRequest.headers['Content-MD5'] = md5;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.computeSseCustomerKeyMd5"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>computeSseCustomerKeyMd5 (req)](#apidoc.element.vogels.AWS.S3.prototype.computeSseCustomerKeyMd5)
- description and source-code
```javascript
function computeSseCustomerKeyMd5(req) {
  var keys = {
    SSECustomerKey: 'x-amz-server-side-encryption-customer-key-MD5',
    CopySourceSSECustomerKey: 'x-amz-copy-source-server-side-encryption-customer-key-MD5'
  };
  AWS.util.each(keys, function(key, header) {
    if (req.params[key]) {
      var value = AWS.util.crypto.md5(req.params[key], 'base64');
      req.httpRequest.headers[header] = value;
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.S3.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.createBucket"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>createBucket (params, callback)](#apidoc.element.vogels.AWS.S3.prototype.createBucket)
- description and source-code
```javascript
function createBucket(params, callback) {
  // When creating a bucket *outside* the classic region, the location
  // constraint must be set for the bucket and it must match the endpoint.
  // This chunk of code will set the location constraint param based
  // on the region (when possible), but it will not override a passed-in
  // location constraint.
  if (typeof params === 'function' || !params) {
    callback = callback || params;
    params = {};
  }
  var hostname = this.endpoint.hostname;
  if (hostname !== this.api.globalEndpoint && !params.CreateBucketConfiguration) {
    params.CreateBucketConfiguration = { LocationConstraint: this.config.region };
  }
  return this.makeRequest('createBucket', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.dnsCompatibleBucketName"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>dnsCompatibleBucketName (bucketName)](#apidoc.element.vogels.AWS.S3.prototype.dnsCompatibleBucketName)
- description and source-code
```javascript
function dnsCompatibleBucketName(bucketName) {
  var b = bucketName;
  var domain = new RegExp(/^[a-z0-9][a-z0-9\.\-]{1,61}[a-z0-9]$/);
  var ipAddress = new RegExp(/(\d+\.){3}\d+/);
  var dots = new RegExp(/\.\./);
  return (b.match(domain) && !b.match(ipAddress) && !b.match(dots)) ? true : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.extractData"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>extractData (resp)](#apidoc.element.vogels.AWS.S3.prototype.extractData)
- description and source-code
```javascript
function extractData(resp) {
  var req = resp.request;
  if (req.operation === 'getBucketLocation') {
    var match = resp.httpResponse.body.toString().match(/>(.+)<\/Location/);
    delete resp.data['_'];
    if (match) {
      resp.data.LocationConstraint = match[1];
    } else {
      resp.data.LocationConstraint = '';
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.extractError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>extractError (resp)](#apidoc.element.vogels.AWS.S3.prototype.extractError)
- description and source-code
```javascript
function extractError(resp) {
  var codes = {
    304: 'NotModified',
    403: 'Forbidden',
    400: 'BadRequest',
    404: 'NotFound'
  };

  var code = resp.httpResponse.statusCode;
  var body = resp.httpResponse.body || '';
  var requestId = resp.requestId;
  var extendedRequestId = resp.httpResponse.headers ? resp.httpResponse.headers['x-amz-id-2'] : null;
  if (codes[code] && body.length === 0) {
    resp.error = AWS.util.error(new Error(), {
      code: codes[resp.httpResponse.statusCode],
      message: null
    });
  } else {
    var data = new AWS.XML.Parser().parse(body.toString());
    resp.error = AWS.util.error(new Error(), {
      code: data.Code || code,
      message: data.Message || null,
      region: data.Region || null
    });
  }
  resp.error.requestId = requestId || null;
  resp.error.extendedRequestId = extendedRequestId || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.getSignedUrl"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>getSignedUrl (operation, params, callback)](#apidoc.element.vogels.AWS.S3.prototype.getSignedUrl)
- description and source-code
```javascript
function getSignedUrl(operation, params, callback) {
  params = AWS.util.copy(params || {});
  var expires = params.Expires || 900;
  delete params.Expires; // we can't validate this
  var request = this.makeRequest(operation, params);
  return request.presign(expires, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.noPresignedContentLength"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>noPresignedContentLength (request)](#apidoc.element.vogels.AWS.S3.prototype.noPresignedContentLength)
- description and source-code
```javascript
function noPresignedContentLength(request) {
  if (request.params.ContentLength !== undefined) {
    throw AWS.util.error(new Error(), {code: 'UnexpectedParameter',
      message: 'ContentLength is not supported in pre-signed URLs.'});
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.pathStyleBucketName"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>pathStyleBucketName (bucketName)](#apidoc.element.vogels.AWS.S3.prototype.pathStyleBucketName)
- description and source-code
```javascript
function pathStyleBucketName(bucketName) {
  // user can force path style requests via the configuration
  if (this.config.s3ForcePathStyle) return true;
  if (this.config.s3BucketEndpoint) return false;

  if (this.dnsCompatibleBucketName(bucketName)) {
    return (this.config.sslEnabled && bucketName.match(/\./)) ? true : false;
  } else {
    return true; // not dns compatible names must always use path style
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.populateURI"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>populateURI (req)](#apidoc.element.vogels.AWS.S3.prototype.populateURI)
- description and source-code
```javascript
function populateURI(req) {
  var httpRequest = req.httpRequest;
  var b = req.params.Bucket;

  if (b) {
    if (!req.service.pathStyleBucketName(b)) {
      if (!req.service.config.s3BucketEndpoint) {
        httpRequest.endpoint.hostname =
          b + '.' + httpRequest.endpoint.hostname;

        var port = httpRequest.endpoint.port;
        if (port !== 80 && port !== 443) {
          httpRequest.endpoint.host = httpRequest.endpoint.hostname + ':' +
            httpRequest.endpoint.port;
        } else {
          httpRequest.endpoint.host = httpRequest.endpoint.hostname;
        }
      }

      httpRequest.virtualHostedBucket = b; // needed for signing the request
      httpRequest.path = httpRequest.path.replace(new RegExp('/' + b), '');
      if (httpRequest.path[0] !== '/') {
        httpRequest.path = '/' + httpRequest.path;
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.prepareSignedUrl"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>prepareSignedUrl (request)](#apidoc.element.vogels.AWS.S3.prototype.prepareSignedUrl)
- description and source-code
```javascript
function prepareSignedUrl(request) {
  request.addListener('validate', request.service.noPresignedContentLength);
  request.removeListener('build', request.service.addContentType);
  if (!request.params.Body) {
    // no Content-MD5/SHA-256 if body is not provided
    request.removeListener('build', request.service.computeContentMd5);
  } else {
    request.addListener('afterBuild', AWS.EventListeners.Core.COMPUTE_SHA256);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.retryableError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>retryableError (error, request)](#apidoc.element.vogels.AWS.S3.prototype.retryableError)
- description and source-code
```javascript
function retryableError(error, request) {
  if (operationsWith200StatusCodeError[request.operation] &&
      error.statusCode === 200) {
    return true;
  } else if (error && error.code === 'RequestTimeout') {
    return true;
  } else if (error && error.code === 'AuthorizationHeaderMalformed' &&
      error.region && error.region != request.httpRequest.region) {
    request.httpRequest.region = error.region;
    return true;
  } else {
    var _super = AWS.Service.prototype.retryableError;
    return _super.call(this, error, request);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.S3.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.addListener('validate', this.validateScheme);
  request.addListener('validate', this.validateBucketEndpoint);
  request.addListener('build', this.addContentType);
  request.addListener('build', this.populateURI);
  request.addListener('build', this.computeContentMd5);
  request.addListener('build', this.computeSseCustomerKeyMd5);
  request.addListener('afterBuild', this.addExpect100Continue);
  request.removeListener('validate',
    AWS.EventListeners.Core.VALIDATE_REGION);
  request.addListener('extractError', this.extractError);
  request.addListener('extractData', this.extractData);
  request.addListener('extractData', AWS.util.hoistPayloadMember);
  request.addListener('beforePresign', this.prepareSignedUrl);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.successfulResponse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>successfulResponse (resp)](#apidoc.element.vogels.AWS.S3.prototype.successfulResponse)
- description and source-code
```javascript
function successfulResponse(resp) {
  var req = resp.request;
  var httpResponse = resp.httpResponse;
  if (operationsWith200StatusCodeError[req.operation] &&
      httpResponse.body.toString().match('<Error>')) {
    return false;
  } else {
    return httpResponse.statusCode < 300;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.upload"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>upload (params, options, callback)](#apidoc.element.vogels.AWS.S3.prototype.upload)
- description and source-code
```javascript
function upload(params, options, callback) {
  if (typeof options === 'function' && callback === undefined) {
    callback = options;
    options = null;
  }

  options = options || {};
  options = AWS.util.merge(options || {}, {service: this, params: params});

  var uploader = new AWS.S3.ManagedUpload(options);
  if (typeof callback === 'function') uploader.send(callback);
  return uploader;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.validateBucketEndpoint"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>validateBucketEndpoint (req)](#apidoc.element.vogels.AWS.S3.prototype.validateBucketEndpoint)
- description and source-code
```javascript
validateBucketEndpoint = function (req) {
  if (!req.params.Bucket && req.service.config.s3BucketEndpoint) {
    var msg = 'Cannot send requests to root API with 's3BucketEndpoint' set.';
    throw AWS.util.error(new Error(),
      { code: 'ConfigError', message: msg });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.validateScheme"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>validateScheme (req)](#apidoc.element.vogels.AWS.S3.prototype.validateScheme)
- description and source-code
```javascript
validateScheme = function (req) {
  var params = req.params,
      scheme = req.httpRequest.endpoint.protocol,
      sensitive = params.SSECustomerKey || params.CopySourceSSECustomerKey;
  if (sensitive && scheme !== 'https:') {
    var msg = 'Cannot send SSE keys over HTTP. Set \'sslEnabled\'' +
      'to \'true\' in your configuration';
    throw AWS.util.error(new Error(),
      { code: 'ConfigError', message: msg });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.validateService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.S3.prototype.validateService)
- description and source-code
```javascript
function validateService() {
  // default to us-east-1 when no region is provided
  if (!this.config.region) this.config.region = 'us-east-1';

  if (!this.config.endpoint && this.config.s3BucketEndpoint) {
    var msg = 'An endpoint must be provided when configuring ' +
              ''s3BucketEndpoint' to true.';
    throw AWS.util.error(new Error(),
      {name: 'InvalidEndpoint', message: msg});
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.S3.prototype.willComputeChecksums"></a>[function <span class="apidocSignatureSpan">vogels.AWS.S3.prototype.</span>willComputeChecksums (req)](#apidoc.element.vogels.AWS.S3.prototype.willComputeChecksums)
- description and source-code
```javascript
function willComputeChecksums(req) {
  if (this.computableChecksumOperations[req.operation]) return true;
  if (!this.config.computeChecksums) return false;

  // TODO: compute checksums for Stream objects
  if (!AWS.util.Buffer.isBuffer(req.httpRequest.body) &&
      typeof req.httpRequest.body !== 'string') {
    return false;
  }

  var rules = req.service.api.operations[req.operation].input.members;

  // V4 signer uses SHA256 signatures so only compute MD5 if it is required
  if (req.service.getSignerClass(req) === AWS.Signers.V4) {
    if (rules.ContentMD5 && !rules.ContentMD5.required) return false;
  }

  if (rules.ContentMD5 && !req.params.ContentMD5) return true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SAMLCredentials"></a>[module vogels.AWS.SAMLCredentials](#apidoc.module.vogels.AWS.SAMLCredentials)

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials.SAMLCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SAMLCredentials (params)](#apidoc.element.vogels.AWS.SAMLCredentials.SAMLCredentials)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.SAMLCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SAMLCredentials.prototype"></a>[module vogels.AWS.SAMLCredentials.prototype](#apidoc.module.vogels.AWS.SAMLCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.SAMLCredentials.prototype.constructor)
- description and source-code
```javascript
function SAMLCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials.prototype.createClients"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.SAMLCredentials.prototype.createClients)
- description and source-code
```javascript
createClients = function () {
  this.service = this.service || new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SAMLCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SAMLCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.SAMLCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  self.createClients();
  if (!callback) callback = function(err) { if (err) throw err; };

  self.service.assumeRoleWithSAML(function (err, data) {
    if (!err) {
      self.service.credentialsFrom(data, self);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SES"></a>[module vogels.AWS.SES](#apidoc.module.vogels.AWS.SES)

#### <a name="apidoc.element.vogels.AWS.SES.SES"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SES ()](#apidoc.element.vogels.AWS.SES.SES)
- description and source-code
```javascript
SES = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SES.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SES.</span>__super__ (config)](#apidoc.element.vogels.AWS.SES.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SES.prototype"></a>[module vogels.AWS.SES.prototype](#apidoc.module.vogels.AWS.SES.prototype)

#### <a name="apidoc.element.vogels.AWS.SES.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SES.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SES.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SNS"></a>[module vogels.AWS.SNS](#apidoc.module.vogels.AWS.SNS)

#### <a name="apidoc.element.vogels.AWS.SNS.SNS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SNS ()](#apidoc.element.vogels.AWS.SNS.SNS)
- description and source-code
```javascript
SNS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SNS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SNS.</span>__super__ (config)](#apidoc.element.vogels.AWS.SNS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SNS.prototype"></a>[module vogels.AWS.SNS.prototype](#apidoc.module.vogels.AWS.SNS.prototype)

#### <a name="apidoc.element.vogels.AWS.SNS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SNS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SNS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SQS"></a>[module vogels.AWS.SQS](#apidoc.module.vogels.AWS.SQS)

#### <a name="apidoc.element.vogels.AWS.SQS.SQS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SQS ()](#apidoc.element.vogels.AWS.SQS.SQS)
- description and source-code
```javascript
SQS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.</span>__super__ (config)](#apidoc.element.vogels.AWS.SQS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SQS.prototype"></a>[module vogels.AWS.SQS.prototype](#apidoc.module.vogels.AWS.SQS.prototype)

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.buildEndpoint"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>buildEndpoint (request)](#apidoc.element.vogels.AWS.SQS.prototype.buildEndpoint)
- description and source-code
```javascript
function buildEndpoint(request) {
  var url = request.httpRequest.params.QueueUrl;
  if (url) {
    request.httpRequest.endpoint = new AWS.Endpoint(url);

    // signature version 4 requires the region name to be set,
    // sqs queue urls contain the region name
    var matches = request.httpRequest.endpoint.host.match(/^sqs\.(.+?)\./);
    if (matches) request.httpRequest.region = matches[1];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.calculateChecksum"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>calculateChecksum (data)](#apidoc.element.vogels.AWS.SQS.prototype.calculateChecksum)
- description and source-code
```javascript
function calculateChecksum(data) {
  return AWS.util.crypto.md5(data, 'hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SQS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.isChecksumValid"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>isChecksumValid (checksum, data)](#apidoc.element.vogels.AWS.SQS.prototype.isChecksumValid)
- description and source-code
```javascript
function isChecksumValid(checksum, data) {
  return this.calculateChecksum(data) === checksum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>setupRequestListeners (request)](#apidoc.element.vogels.AWS.SQS.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners(request) {
  request.addListener('build', this.buildEndpoint);

  if (request.service.config.computeChecksums) {
    if (request.operation === 'sendMessage') {
      request.addListener('extractData', this.verifySendMessageChecksum);
    } else if (request.operation === 'sendMessageBatch') {
      request.addListener('extractData', this.verifySendMessageBatchChecksum);
    } else if (request.operation === 'receiveMessage') {
      request.addListener('extractData', this.verifyReceiveMessageChecksum);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.throwInvalidChecksumError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>throwInvalidChecksumError (response, ids, message)](#apidoc.element.vogels.AWS.SQS.prototype.throwInvalidChecksumError)
- description and source-code
```javascript
function throwInvalidChecksumError(response, ids, message) {
  response.error = AWS.util.error(new Error(), {
    retryable: true,
    code: 'InvalidChecksum',
    messageIds: ids,
    message: response.request.operation +
             ' returned an invalid MD5 response. ' + message
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.verifyReceiveMessageChecksum"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>verifyReceiveMessageChecksum (response)](#apidoc.element.vogels.AWS.SQS.prototype.verifyReceiveMessageChecksum)
- description and source-code
```javascript
function verifyReceiveMessageChecksum(response) {
  if (!response.data) return;

  var service = this.service;
  var messageIds = [];
  AWS.util.arrayEach(response.data.Messages, function(message) {
    var md5 = message.MD5OfBody;
    var body = message.Body;
    if (!service.isChecksumValid(md5, body)) {
      messageIds.push(message.MessageId);
    }
  });

  if (messageIds.length > 0) {
    service.throwInvalidChecksumError(response, messageIds,
      'Invalid messages: ' + messageIds.join(', '));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.verifySendMessageBatchChecksum"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>verifySendMessageBatchChecksum (response)](#apidoc.element.vogels.AWS.SQS.prototype.verifySendMessageBatchChecksum)
- description and source-code
```javascript
function verifySendMessageBatchChecksum(response) {
  if (!response.data) return;

  var service = this.service;
  var entries = {};
  var errors = [];
  var messageIds = [];
  AWS.util.arrayEach(response.data.Successful, function (entry) {
    entries[entry.Id] = entry;
  });
  AWS.util.arrayEach(this.params.Entries, function (entry) {
    if (entries[entry.Id]) {
      var md5 = entries[entry.Id].MD5OfMessageBody;
      var body = entry.MessageBody;
      if (!service.isChecksumValid(md5, body)) {
        errors.push(entry.Id);
        messageIds.push(entries[entry.Id].MessageId);
      }
    }
  });

  if (errors.length > 0) {
    service.throwInvalidChecksumError(response, messageIds,
      'Invalid messages: ' + errors.join(', '));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SQS.prototype.verifySendMessageChecksum"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SQS.prototype.</span>verifySendMessageChecksum (response)](#apidoc.element.vogels.AWS.SQS.prototype.verifySendMessageChecksum)
- description and source-code
```javascript
function verifySendMessageChecksum(response) {
  if (!response.data) return;

  var md5 = response.data.MD5OfMessageBody;
  var body = this.params.MessageBody;
  var calculatedMd5 = this.service.calculateChecksum(body);
  if (calculatedMd5 !== md5) {
    var msg = 'Got "' + response.data.MD5OfMessageBody +
      '", expecting "' + calculatedMd5 + '".';
    this.service.throwInvalidChecksumError(response,
      [response.data.MessageId], msg);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SSM"></a>[module vogels.AWS.SSM](#apidoc.module.vogels.AWS.SSM)

#### <a name="apidoc.element.vogels.AWS.SSM.SSM"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SSM ()](#apidoc.element.vogels.AWS.SSM.SSM)
- description and source-code
```javascript
SSM = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SSM.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SSM.</span>__super__ (config)](#apidoc.element.vogels.AWS.SSM.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SSM.prototype"></a>[module vogels.AWS.SSM.prototype](#apidoc.module.vogels.AWS.SSM.prototype)

#### <a name="apidoc.element.vogels.AWS.SSM.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SSM.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SSM.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.STS"></a>[module vogels.AWS.STS](#apidoc.module.vogels.AWS.STS)

#### <a name="apidoc.element.vogels.AWS.STS.STS"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>STS ()](#apidoc.element.vogels.AWS.STS.STS)
- description and source-code
```javascript
STS = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.STS.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.STS.</span>__super__ (config)](#apidoc.element.vogels.AWS.STS.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.STS.prototype"></a>[module vogels.AWS.STS.prototype](#apidoc.module.vogels.AWS.STS.prototype)

#### <a name="apidoc.element.vogels.AWS.STS.prototype.assumeRoleWithSAML"></a>[function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>assumeRoleWithSAML (params, callback)](#apidoc.element.vogels.AWS.STS.prototype.assumeRoleWithSAML)
- description and source-code
```javascript
function assumeRoleWithSAML(params, callback) {
  return this.makeUnauthenticatedRequest('assumeRoleWithSAML', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.STS.prototype.assumeRoleWithWebIdentity"></a>[function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>assumeRoleWithWebIdentity (params, callback)](#apidoc.element.vogels.AWS.STS.prototype.assumeRoleWithWebIdentity)
- description and source-code
```javascript
function assumeRoleWithWebIdentity(params, callback) {
  return this.makeUnauthenticatedRequest('assumeRoleWithWebIdentity', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.STS.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.STS.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.STS.prototype.credentialsFrom"></a>[function <span class="apidocSignatureSpan">vogels.AWS.STS.prototype.</span>credentialsFrom (data, credentials)](#apidoc.element.vogels.AWS.STS.prototype.credentialsFrom)
- description and source-code
```javascript
function credentialsFrom(data, credentials) {
  if (!data) return null;
  if (!credentials) credentials = new AWS.TemporaryCredentials();
  credentials.expired = false;
  credentials.accessKeyId = data.Credentials.AccessKeyId;
  credentials.secretAccessKey = data.Credentials.SecretAccessKey;
  credentials.sessionToken = data.Credentials.SessionToken;
  credentials.expireTime = data.Credentials.Expiration;
  return credentials;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SWF"></a>[module vogels.AWS.SWF](#apidoc.module.vogels.AWS.SWF)

#### <a name="apidoc.element.vogels.AWS.SWF.SWF"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SWF ()](#apidoc.element.vogels.AWS.SWF.SWF)
- description and source-code
```javascript
SWF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SWF.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SWF.</span>__super__ (config)](#apidoc.element.vogels.AWS.SWF.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SWF.prototype"></a>[module vogels.AWS.SWF.prototype](#apidoc.module.vogels.AWS.SWF.prototype)

#### <a name="apidoc.element.vogels.AWS.SWF.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SWF.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SWF.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SequentialExecutor"></a>[module vogels.AWS.SequentialExecutor](#apidoc.module.vogels.AWS.SequentialExecutor)

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.SequentialExecutor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SequentialExecutor ()](#apidoc.element.vogels.AWS.SequentialExecutor.SequentialExecutor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.</span>__super__ ()](#apidoc.element.vogels.AWS.SequentialExecutor.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SequentialExecutor.prototype"></a>[module vogels.AWS.SequentialExecutor.prototype](#apidoc.module.vogels.AWS.SequentialExecutor.prototype)

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.addListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addListener (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addListener)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.addListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addListeners (listeners)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addListeners)
- description and source-code
```javascript
function addListeners(listeners) {
  var self = this;

  // extract listeners if parameter is an SequentialExecutor object
  if (listeners._events) listeners = listeners._events;

  AWS.util.each(listeners, function(event, callbacks) {
    if (typeof callbacks === 'function') callbacks = [callbacks];
    AWS.util.arrayEach(callbacks, function(callback) {
      self.on(event, callback);
    });
  });

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedAsyncListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addNamedAsyncListener (name, eventName, callback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedAsyncListener)
- description and source-code
```javascript
function addNamedAsyncListener(name, eventName, callback) {
  callback._isAsync = true;
  return this.addNamedListener(name, eventName, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addNamedListener (name, eventName, callback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedListener)
- description and source-code
```javascript
function addNamedListener(name, eventName, callback) {
  this[name] = callback;
  this.addListener(eventName, callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>addNamedListeners (callback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.addNamedListeners)
- description and source-code
```javascript
function addNamedListeners(callback) {
  var self = this;
  callback(
    function() {
      self.addNamedListener.apply(self, arguments);
    },
    function() {
      self.addNamedAsyncListener.apply(self, arguments);
    }
  );
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.callListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>callListeners (listeners, args, doneCallback, prevError)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.callListeners)
- description and source-code
```javascript
function callListeners(listeners, args, doneCallback, prevError) {
  var self = this;
  var error = prevError || null;

  function callNextListener(err) {
    if (err) {
      error = AWS.util.error(error || new Error(), err);
      if (self._haltHandlersOnError) {
        return doneCallback.call(self, error);
      }
    }
    self.callListeners(listeners, args, doneCallback, error);
  }

  while (listeners.length > 0) {
    var listener = listeners.shift();
    if (listener._isAsync) { // asynchronous listener
      listener.apply(self, args.concat([callNextListener]));
      return; // stop here, callNextListener will continue
    } else { // synchronous listener
      try {
        listener.apply(self, args);
      } catch (err) {
        error = AWS.util.error(error || new Error(), err);
      }
      if (error && self._haltHandlersOnError) {
        doneCallback.call(self, error);
        return;
      }
    }
  }
  doneCallback.call(self, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.constructor)
- description and source-code
```javascript
function SequentialExecutor() {
  this._events = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.emit"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>emit (eventName, eventArgs, doneCallback)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.emit)
- description and source-code
```javascript
function emit(eventName, eventArgs, doneCallback) {
  if (!doneCallback) doneCallback = function() { };
  var listeners = this.listeners(eventName);
  var count = listeners.length;
  this.callListeners(listeners, eventArgs, doneCallback);
  return count > 0;
}
```
- example usage
```shell
...
var streamMode = false;
var combinedStream = new Readable({objectMode: true});

if(!callback) {
  streamMode = true;
  callback = function (err) {
    if(err) {
      combinedStream.emit('error', err);
    }
  };
}

var scanFuncs = [];
_.times(self.totalSegments, function(segment) {
  var scn = new Scan(self.table, self.serializer);
...
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.listeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>listeners (eventName)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.listeners)
- description and source-code
```javascript
function listeners(eventName) {
  return this._events[eventName] ? this._events[eventName].slice(0) : [];
}
```
- example usage
```shell
...
  }

  return callback(null, item);
});
};

internals.callBeforeHooks = function (table, name, startFun, callback) {
var listeners = table._before.listeners(name);

return async.waterfall([startFun].concat(listeners), callback);
};

Table.prototype.create = function (item, options, callback) {
var self = this;
...
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.on"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>on (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.on)
- description and source-code
```javascript
function on(eventName, listener) {
  if (this._events[eventName]) {
    this._events[eventName].push(listener);
  } else {
    this._events[eventName] = [listener];
  }
  return this;
}
```
- example usage
```shell
...
### Streaming api
vogels supports a basic streaming api in addition to the callback
api for 'query', 'scan', and 'parallelScan' operations.

'''js
var stream = Account.parallelScan(4).exec();

stream.on('readable', function () {
  console.log('single parallel scan response', stream.read());
});

stream.on('end', function () {
  console.log('Parallel scan of accounts finished');
});
...
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.onAsync"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>onAsync (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.onAsync)
- description and source-code
```javascript
function onAsync(eventName, listener) {
  listener._isAsync = true;
  return this.on(eventName, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>removeAllListeners (eventName)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(eventName) {
  if (eventName) {
    delete this._events[eventName];
  } else {
    this._events = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SequentialExecutor.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SequentialExecutor.prototype.</span>removeListener (eventName, listener)](#apidoc.element.vogels.AWS.SequentialExecutor.prototype.removeListener)
- description and source-code
```javascript
function removeListener(eventName, listener) {
  var listeners = this._events[eventName];
  if (listeners) {
    var length = listeners.length;
    var position = -1;
    for (var i = 0; i < length; ++i) {
      if (listeners[i] === listener) {
        position = i;
      }
    }
    if (position > -1) {
      listeners.splice(position, 1);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Service"></a>[module vogels.AWS.Service](#apidoc.module.vogels.AWS.Service)

#### <a name="apidoc.element.vogels.AWS.Service.Service"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Service (config)](#apidoc.element.vogels.AWS.Service.Service)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>__super__ ()](#apidoc.element.vogels.AWS.Service.__super__)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.addVersions"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>addVersions (svc, versions)](#apidoc.element.vogels.AWS.Service.addVersions)
- description and source-code
```javascript
function addVersions(svc, versions) {
  if (!Array.isArray(versions)) versions = [versions];

  svc.services = svc.services || {};
  for (var i = 0; i < versions.length; i++) {
    if (svc.services[versions[i]] === undefined) {
      svc.services[versions[i]] = null;
    }
  }

  svc.apiVersions = Object.keys(svc.services).sort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.defineMethods"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>defineMethods (svc)](#apidoc.element.vogels.AWS.Service.defineMethods)
- description and source-code
```javascript
function defineMethods(svc) {
  AWS.util.each(svc.prototype.api.operations, function iterator(method) {
    if (svc.prototype[method]) return;
    svc.prototype[method] = function (params, callback) {
      return this.makeRequest(method, params, callback);
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.defineService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>defineService (serviceIdentifier, versions, features)](#apidoc.element.vogels.AWS.Service.defineService)
- description and source-code
```javascript
function defineService(serviceIdentifier, versions, features) {
  AWS.Service._serviceMap[serviceIdentifier] = true;
  if (!Array.isArray(versions)) {
    features = versions;
    versions = [];
  }

  var svc = inherit(AWS.Service, features || {});

  if (typeof serviceIdentifier === 'string') {
    AWS.Service.addVersions(svc, versions);

    var identifier = svc.serviceIdentifier || serviceIdentifier;
    svc.serviceIdentifier = identifier;
  } else { // defineService called with an API
    svc.prototype.api = serviceIdentifier;
    AWS.Service.defineMethods(svc);
  }

  return svc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.defineServiceApi"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>defineServiceApi (superclass, version, apiConfig)](#apidoc.element.vogels.AWS.Service.defineServiceApi)
- description and source-code
```javascript
function defineServiceApi(superclass, version, apiConfig) {
  var svc = inherit(superclass, {
    serviceIdentifier: superclass.serviceIdentifier
  });

  function setApi(api) {
    if (api.isApi) {
      svc.prototype.api = api;
    } else {
      svc.prototype.api = new Api(api);
    }
  }

  if (typeof version === 'string') {
    if (apiConfig) {
      setApi(apiConfig);
    } else {
      try {
        setApi(AWS.apiLoader(superclass.serviceIdentifier, version));
      } catch (err) {
        throw AWS.util.error(err, {
          message: 'Could not find API configuration ' +
            superclass.serviceIdentifier + '-' + version
        });
      }
    }
    if (!superclass.services.hasOwnProperty(version)) {
      superclass.apiVersions = superclass.apiVersions.concat(version).sort();
    }
    superclass.services[version] = svc;
  } else {
    setApi(version);
  }

  AWS.Service.defineMethods(svc);
  return svc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.hasService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.</span>hasService (identifier)](#apidoc.element.vogels.AWS.Service.hasService)
- description and source-code
```javascript
hasService = function (identifier) {
  return AWS.Service._serviceMap.hasOwnProperty(identifier);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Service.prototype"></a>[module vogels.AWS.Service.prototype](#apidoc.module.vogels.AWS.Service.prototype)

#### <a name="apidoc.element.vogels.AWS.Service.prototype.addAllRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>addAllRequestListeners (request)](#apidoc.element.vogels.AWS.Service.prototype.addAllRequestListeners)
- description and source-code
```javascript
function addAllRequestListeners(request) {
  var list = [AWS.events, AWS.EventListeners.Core, this.serviceInterface(),
              AWS.EventListeners.CorePost];
  for (var i = 0; i < list.length; i++) {
    if (list[i]) request.addListeners(list[i]);
  }

  // disable parameter validation
  if (!this.config.paramValidation) {
    request.removeListener('validate',
      AWS.EventListeners.Core.VALIDATE_PARAMETERS);
  }

  if (this.config.logger) { // add logging events
    request.addListeners(AWS.EventListeners.Logger);
  }

  this.setupRequestListeners(request);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.clockSkewError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>clockSkewError (error)](#apidoc.element.vogels.AWS.Service.prototype.clockSkewError)
- description and source-code
```javascript
function clockSkewError(error) {
  switch (error.code) {
    case 'RequestTimeTooSkewed':
    case 'RequestExpired':
    case 'InvalidSignatureException':
    case 'SignatureDoesNotMatch':
    case 'AuthFailure':
    case 'RequestInTheFuture':
      return true;
    default: return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>constructor (config)](#apidoc.element.vogels.AWS.Service.prototype.constructor)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.endpointFromTemplate"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>endpointFromTemplate (endpoint)](#apidoc.element.vogels.AWS.Service.prototype.endpointFromTemplate)
- description and source-code
```javascript
function endpointFromTemplate(endpoint) {
  if (typeof endpoint !== 'string') return endpoint;

  var e = endpoint;
  e = e.replace(/\{service\}/g, this.api.endpointPrefix);
  e = e.replace(/\{region\}/g, this.config.region);
  e = e.replace(/\{scheme\}/g, this.config.sslEnabled ? 'https' : 'http');
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.expiredCredentialsError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>expiredCredentialsError (error)](#apidoc.element.vogels.AWS.Service.prototype.expiredCredentialsError)
- description and source-code
```javascript
function expiredCredentialsError(error) {
  // TODO : this only handles *one* of the expired credential codes
  return (error.code === 'ExpiredTokenException');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.getLatestServiceClass"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>getLatestServiceClass (version)](#apidoc.element.vogels.AWS.Service.prototype.getLatestServiceClass)
- description and source-code
```javascript
function getLatestServiceClass(version) {
  version = this.getLatestServiceVersion(version);
  if (this.constructor.services[version] === null) {
    AWS.Service.defineServiceApi(this.constructor, version);
  }

  return this.constructor.services[version];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.getLatestServiceVersion"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>getLatestServiceVersion (version)](#apidoc.element.vogels.AWS.Service.prototype.getLatestServiceVersion)
- description and source-code
```javascript
function getLatestServiceVersion(version) {
  if (!this.constructor.services || this.constructor.services.length === 0) {
    throw new Error('No services defined on ' +
                    this.constructor.serviceIdentifier);
  }

  if (!version) {
    version = 'latest';
  } else if (AWS.util.isType(version, Date)) {
    version = AWS.util.date.iso8601(version).split('T')[0];
  }

  if (Object.hasOwnProperty(this.constructor.services, version)) {
    return version;
  }

  var keys = Object.keys(this.constructor.services).sort();
  var selectedVersion = null;
  for (var i = keys.length - 1; i >= 0; i--) {
    // versions that end in "*" are not available on disk and can be
    // skipped, so do not choose these as selectedVersions
    if (keys[i][keys[i].length - 1] !== '*') {
      selectedVersion = keys[i];
    }
    if (keys[i].substr(0, 10) <= version) {
      return selectedVersion;
    }
  }

  throw new Error('Could not find ' + this.constructor.serviceIdentifier +
                  ' API to satisfy version constraint '' + version + '\'');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.getSignerClass"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>getSignerClass ()](#apidoc.element.vogels.AWS.Service.prototype.getSignerClass)
- description and source-code
```javascript
function getSignerClass() {
  var version;
  if (this.config.signatureVersion) {
    version = this.config.signatureVersion;
  } else {
    version = this.api.signatureVersion;
  }
  return AWS.Signers.RequestSigner.getVersion(version);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.initialize"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>initialize (config)](#apidoc.element.vogels.AWS.Service.prototype.initialize)
- description and source-code
```javascript
function initialize(config) {
  var svcConfig = AWS.config[this.serviceIdentifier];

  this.config = new AWS.Config(AWS.config);
  if (svcConfig) this.config.update(svcConfig, true);
  if (config) this.config.update(config, true);

  this.validateService();
  if (!this.config.endpoint) regionConfig(this);

  this.config.endpoint = this.endpointFromTemplate(this.config.endpoint);
  this.setEndpoint(this.config.endpoint);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.loadServiceClass"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>loadServiceClass (serviceConfig)](#apidoc.element.vogels.AWS.Service.prototype.loadServiceClass)
- description and source-code
```javascript
function loadServiceClass(serviceConfig) {
  var config = serviceConfig;
  if (!AWS.util.isEmpty(this.api)) {
    return null;
  } else if (config.apiConfig) {
    return AWS.Service.defineServiceApi(this.constructor, config.apiConfig);
  } else if (!this.constructor.services) {
    return null;
  } else {
    config = new AWS.Config(AWS.config);
    config.update(serviceConfig, true);
    var version = config.apiVersions[this.constructor.serviceIdentifier];
    version = version || config.apiVersion;
    return this.getLatestServiceClass(version);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.makeRequest"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>makeRequest (operation, params, callback)](#apidoc.element.vogels.AWS.Service.prototype.makeRequest)
- description and source-code
```javascript
function makeRequest(operation, params, callback) {
  if (typeof params === 'function') {
    callback = params;
    params = null;
  }

  params = params || {};
  if (this.config.params) { // copy only toplevel bound params
    var rules = this.api.operations[operation];
    if (rules) {
      params = AWS.util.copy(params);
      AWS.util.each(this.config.params, function(key, value) {
        if (rules.input.members[key]) {
          if (params[key] === undefined || params[key] === null) {
            params[key] = value;
          }
        }
      });
    }
  }

  var request = new AWS.Request(this, operation, params);
  this.addAllRequestListeners(request);

  if (callback) request.send(callback);
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.makeUnauthenticatedRequest"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>makeUnauthenticatedRequest (operation, params, callback)](#apidoc.element.vogels.AWS.Service.prototype.makeUnauthenticatedRequest)
- description and source-code
```javascript
function makeUnauthenticatedRequest(operation, params, callback) {
  if (typeof params === 'function') {
    callback = params;
    params = {};
  }

  var request = this.makeRequest(operation, params).toUnauthenticated();
  return callback ? request.send(callback) : request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.networkingError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>networkingError (error)](#apidoc.element.vogels.AWS.Service.prototype.networkingError)
- description and source-code
```javascript
function networkingError(error) {
  return error.code === 'NetworkingError';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.numRetries"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>numRetries ()](#apidoc.element.vogels.AWS.Service.prototype.numRetries)
- description and source-code
```javascript
function numRetries() {
  if (this.config.maxRetries !== undefined) {
    return this.config.maxRetries;
  } else {
    return this.defaultRetryCount;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.paginationConfig"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>paginationConfig (operation, throwException)](#apidoc.element.vogels.AWS.Service.prototype.paginationConfig)
- description and source-code
```javascript
function paginationConfig(operation, throwException) {
  var paginator = this.api.operations[operation].paginator;
  if (!paginator) {
    if (throwException) {
      var e = new Error();
      throw AWS.util.error(e, 'No pagination configuration for ' + operation);
    }
    return null;
  }

  return paginator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.retryDelays"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>retryDelays (retryCount)](#apidoc.element.vogels.AWS.Service.prototype.retryDelays)
- description and source-code
```javascript
function retryDelays(retryCount) {
  var retryDelayOptions = this.config.retryDelayOptions || {};
  var customBackoff = retryDelayOptions.customBackoff || null;
  if (typeof customBackoff === 'function') {
    return customBackoff(retryCount);
  }
  var base = retryDelayOptions.base || 30;
  var delay = Math.random() * (Math.pow(2, retryCount) * base);
  return delay;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.retryableError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>retryableError (error)](#apidoc.element.vogels.AWS.Service.prototype.retryableError)
- description and source-code
```javascript
function retryableError(error) {
  if (this.networkingError(error)) return true;
  if (this.expiredCredentialsError(error)) return true;
  if (this.throttledError(error)) return true;
  if (error.statusCode >= 500) return true;
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.serviceInterface"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>serviceInterface ()](#apidoc.element.vogels.AWS.Service.prototype.serviceInterface)
- description and source-code
```javascript
function serviceInterface() {
  switch (this.api.protocol) {
    case 'ec2': return AWS.EventListeners.Query;
    case 'query': return AWS.EventListeners.Query;
    case 'json': return AWS.EventListeners.Json;
    case 'rest-json': return AWS.EventListeners.RestJson;
    case 'rest-xml': return AWS.EventListeners.RestXml;
  }
  if (this.api.protocol) {
    throw new Error('Invalid service 'protocol\' ' +
      this.api.protocol + ' in API config');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.setEndpoint"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>setEndpoint (endpoint)](#apidoc.element.vogels.AWS.Service.prototype.setEndpoint)
- description and source-code
```javascript
function setEndpoint(endpoint) {
  this.endpoint = new AWS.Endpoint(endpoint, this.config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.setupRequestListeners"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>setupRequestListeners ()](#apidoc.element.vogels.AWS.Service.prototype.setupRequestListeners)
- description and source-code
```javascript
function setupRequestListeners() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.successfulResponse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>successfulResponse (resp)](#apidoc.element.vogels.AWS.Service.prototype.successfulResponse)
- description and source-code
```javascript
function successfulResponse(resp) {
  return resp.httpResponse.statusCode < 300;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.throttledError"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>throttledError (error)](#apidoc.element.vogels.AWS.Service.prototype.throttledError)
- description and source-code
```javascript
function throttledError(error) {
  // this logic varies between services
  switch (error.code) {
    case 'ProvisionedThroughputExceededException':
    case 'Throttling':
    case 'ThrottlingException':
    case 'RequestLimitExceeded':
    case 'RequestThrottled':
      return true;
    default:
      return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.validateService"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>validateService ()](#apidoc.element.vogels.AWS.Service.prototype.validateService)
- description and source-code
```javascript
function validateService() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Service.prototype.waitFor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Service.prototype.</span>waitFor (state, params, callback)](#apidoc.element.vogels.AWS.Service.prototype.waitFor)
- description and source-code
```javascript
function waitFor(state, params, callback) {
  var waiter = new AWS.ResourceWaiter(this, state);
  return waiter.wait(params, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SharedIniFileCredentials"></a>[module vogels.AWS.SharedIniFileCredentials](#apidoc.module.vogels.AWS.SharedIniFileCredentials)

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials.SharedIniFileCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SharedIniFileCredentials (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials.SharedIniFileCredentials)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.SharedIniFileCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SharedIniFileCredentials.prototype"></a>[module vogels.AWS.SharedIniFileCredentials.prototype](#apidoc.module.vogels.AWS.SharedIniFileCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.prototype.</span>constructor (options)](#apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.constructor)
- description and source-code
```javascript
function SharedIniFileCredentials(options) {
  AWS.Credentials.call(this);

  options = options || {};

  this.filename = options.filename;
  this.profile = options.profile || process.env.AWS_PROFILE || 'default';
  this.get(function() {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.loadDefaultFilename"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.prototype.</span>loadDefaultFilename ()](#apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.loadDefaultFilename)
- description and source-code
```javascript
function loadDefaultFilename() {
  var env = process.env;
  var home = env.HOME ||
             env.USERPROFILE ||
             (env.HOMEPATH ? ((env.HOMEDRIVE || 'C:/') + env.HOMEPATH) : null);
  if (!home) {
    throw AWS.util.error(
      new Error('Cannot load credentials, HOME path not set'));
  }

  this.filename = path.join(home, '.aws', 'credentials');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SharedIniFileCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.SharedIniFileCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  if (!callback) callback = function(err) { if (err) throw err; };
  try {
    if (!this.filename) this.loadDefaultFilename();
    var creds = AWS.util.ini.parse(AWS.util.readFileSync(this.filename));
    if (typeof creds[this.profile] === 'object') {
      this.accessKeyId = creds[this.profile]['aws_access_key_id'];
      this.secretAccessKey = creds[this.profile]['aws_secret_access_key'];
      this.sessionToken = creds[this.profile]['aws_session_token'];
    }

    if (!this.accessKeyId || !this.secretAccessKey) {
      throw new Error('Credentials not set in ' + this.filename +
                      ' using profile ' + this.profile);
    }
    this.expired = false;
    callback();
  } catch (err) {
    callback(err);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers"></a>[module vogels.AWS.Signers](#apidoc.module.vogels.AWS.Signers)

#### <a name="apidoc.element.vogels.AWS.Signers.Presign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>Presign ()](#apidoc.element.vogels.AWS.Signers.Presign)
- description and source-code
```javascript
Presign = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.RequestSigner"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>RequestSigner (request)](#apidoc.element.vogels.AWS.Signers.RequestSigner)
- description and source-code
```javascript
function RequestSigner(request) {
  this.request = request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.S3"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>S3 ()](#apidoc.element.vogels.AWS.Signers.S3)
- description and source-code
```javascript
S3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V2"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V2 ()](#apidoc.element.vogels.AWS.Signers.V2)
- description and source-code
```javascript
V2 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V3 ()](#apidoc.element.vogels.AWS.Signers.V3)
- description and source-code
```javascript
V3 = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3Https"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V3Https ()](#apidoc.element.vogels.AWS.Signers.V3Https)
- description and source-code
```javascript
V3Https = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.</span>V4 (request, serviceName, signatureCache)](#apidoc.element.vogels.AWS.Signers.V4)
- description and source-code
```javascript
function V4(request, serviceName, signatureCache) {
  AWS.Signers.RequestSigner.call(this, request);
  this.serviceName = serviceName;
  this.signatureCache = signatureCache;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.Presign.prototype"></a>[module vogels.AWS.Signers.Presign.prototype](#apidoc.module.vogels.AWS.Signers.Presign.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.Presign.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.Presign.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.Presign.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.Presign.prototype.sign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.Presign.prototype.</span>sign (request, expireTime, callback)](#apidoc.element.vogels.AWS.Signers.Presign.prototype.sign)
- description and source-code
```javascript
function sign(request, expireTime, callback) {
  request.httpRequest.headers[expiresHeader] = expireTime || 3600;
  request.on('build', signedUrlBuilder);
  request.on('sign', signedUrlSigner);
  request.removeListener('afterBuild',
    AWS.EventListeners.Core.SET_CONTENT_LENGTH);
  request.removeListener('afterBuild',
    AWS.EventListeners.Core.COMPUTE_SHA256);

  request.emit('beforePresign', [request]);

  if (callback) {
    request.build(function() {
      if (this.response.error) callback(this.response.error);
      else {
        callback(null, AWS.util.urlFormat(request.httpRequest.endpoint));
      }
    });
  } else {
    request.build();
    if (request.response.error) throw request.response.error;
    return AWS.util.urlFormat(request.httpRequest.endpoint);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.RequestSigner.prototype"></a>[module vogels.AWS.Signers.RequestSigner.prototype](#apidoc.module.vogels.AWS.Signers.RequestSigner.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.RequestSigner.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.RequestSigner.prototype.</span>constructor (request)](#apidoc.element.vogels.AWS.Signers.RequestSigner.prototype.constructor)
- description and source-code
```javascript
function RequestSigner(request) {
  this.request = request;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.S3.prototype"></a>[module vogels.AWS.Signers.S3.prototype](#apidoc.module.vogels.AWS.Signers.S3.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.S3.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.S3.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {
  if (!this.request.headers['presigned-expires']) {
    this.request.headers['X-Amz-Date'] = AWS.util.date.rfc822(date);
  }

  if (credentials.sessionToken) {
    // presigned URLs require this header to be lowercased
    this.request.headers['x-amz-security-token'] = credentials.sessionToken;
  }

  var signature = this.sign(credentials.secretAccessKey, this.stringToSign());
  var auth = 'AWS ' + credentials.accessKeyId + ':' + signature;

  this.request.headers['Authorization'] = auth;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.S3.prototype.canonicalizedAmzHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>canonicalizedAmzHeaders ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.canonicalizedAmzHeaders)
- description and source-code
```javascript
function canonicalizedAmzHeaders() {

  var amzHeaders = [];

  AWS.util.each(this.request.headers, function (name) {
    if (name.match(/^x-amz-/i))
      amzHeaders.push(name);
  });

  amzHeaders.sort(function (a, b) {
    return a.toLowerCase() < b.toLowerCase() ? -1 : 1;
  });

  var parts = [];
  AWS.util.arrayEach.call(this, amzHeaders, function (name) {
    parts.push(name.toLowerCase() + ':' + String(this.request.headers[name]));
  });

  return parts.join('\n');

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.S3.prototype.canonicalizedResource"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>canonicalizedResource ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.canonicalizedResource)
- description and source-code
```javascript
function canonicalizedResource() {

  var r = this.request;

  var parts = r.path.split('?');
  var path = parts[0];
  var querystring = parts[1];

  var resource = '';

  if (r.virtualHostedBucket)
    resource += '/' + r.virtualHostedBucket;

  resource += path;

  if (querystring) {

    // collect a list of sub resources and query params that need to be signed
    var resources = [];

    AWS.util.arrayEach.call(this, querystring.split('&'), function (param) {
      var name = param.split('=')[0];
      var value = param.split('=')[1];
      if (this.subResources[name] || this.responseHeaders[name]) {
        var subresource = { name: name };
        if (value !== undefined) {
          if (this.subResources[name]) {
            subresource.value = value;
          } else {
            subresource.value = decodeURIComponent(value);
          }
        }
        resources.push(subresource);
      }
    });

    resources.sort(function (a, b) { return a.name < b.name ? -1 : 1; });

    if (resources.length) {

      querystring = [];
      AWS.util.arrayEach(resources, function (res) {
        if (res.value === undefined) {
          querystring.push(res.name);
        } else {
          querystring.push(res.name + '=' + res.value);
        }
      });

      resource += '?' + querystring.join('&');
    }

  }

  return resource;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.S3.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.S3.prototype.sign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>sign (secret, string)](#apidoc.element.vogels.AWS.Signers.S3.prototype.sign)
- description and source-code
```javascript
function sign(secret, string) {
  return AWS.util.crypto.hmac(secret, string, 'base64', 'sha1');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.S3.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.S3.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.S3.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  var r = this.request;

  var parts = [];
  parts.push(r.method);
  parts.push(r.headers['Content-MD5'] || '');
  parts.push(r.headers['Content-Type'] || '');

  // This is the "Date" header, but we use X-Amz-Date.
  // The S3 signing mechanism requires us to pass an empty
  // string for this Date header regardless.
  parts.push(r.headers['presigned-expires'] || '');

  var headers = this.canonicalizedAmzHeaders();
  if (headers) parts.push(headers);
  parts.push(this.canonicalizedResource());

  return parts.join('\n');

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.V2.prototype"></a>[module vogels.AWS.Signers.V2.prototype](#apidoc.module.vogels.AWS.Signers.V2.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.V2.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.V2.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {

  if (!date) date = AWS.util.date.getDate();

  var r = this.request;

  r.params.Timestamp = AWS.util.date.iso8601(date);
  r.params.SignatureVersion = '2';
  r.params.SignatureMethod = 'HmacSHA256';
  r.params.AWSAccessKeyId = credentials.accessKeyId;

  if (credentials.sessionToken) {
    r.params.SecurityToken = credentials.sessionToken;
  }

  delete r.params.Signature; // delete old Signature for re-signing
  r.params.Signature = this.signature(credentials);

  r.body = AWS.util.queryParamsToString(r.params);
  r.headers['Content-Length'] = r.body.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V2.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.V2.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V2.prototype.signature"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>signature (credentials)](#apidoc.element.vogels.AWS.Signers.V2.prototype.signature)
- description and source-code
```javascript
function signature(credentials) {
  return AWS.util.crypto.hmac(credentials.secretAccessKey, this.stringToSign(), 'base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V2.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V2.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.V2.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  var parts = [];
  parts.push(this.request.method);
  parts.push(this.request.endpoint.host.toLowerCase());
  parts.push(this.request.pathname());
  parts.push(AWS.util.queryParamsToString(this.request.params));
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.V3.prototype"></a>[module vogels.AWS.Signers.V3.prototype](#apidoc.module.vogels.AWS.Signers.V3.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.V3.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {

  var datetime = AWS.util.date.rfc822(date);

  this.request.headers['X-Amz-Date'] = datetime;

  if (credentials.sessionToken) {
    this.request.headers['x-amz-security-token'] = credentials.sessionToken;
  }

  this.request.headers['X-Amzn-Authorization'] =
    this.authorization(credentials, datetime);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.authorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>authorization (credentials)](#apidoc.element.vogels.AWS.Signers.V3.prototype.authorization)
- description and source-code
```javascript
function authorization(credentials) {
  return 'AWS3 ' +
    'AWSAccessKeyId=' + credentials.accessKeyId + ',' +
    'Algorithm=HmacSHA256,' +
    'SignedHeaders=' + this.signedHeaders() + ',' +
    'Signature=' + this.signature(credentials);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.canonicalHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>canonicalHeaders ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.canonicalHeaders)
- description and source-code
```javascript
function canonicalHeaders() {
  var headers = this.request.headers;
  var parts = [];
  AWS.util.arrayEach(this.headersToSign(), function iterator(h) {
    parts.push(h.toLowerCase().trim() + ':' + String(headers[h]).trim());
  });
  return parts.sort().join('\n') + '\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.headersToSign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>headersToSign ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.headersToSign)
- description and source-code
```javascript
function headersToSign() {
  var headers = [];
  AWS.util.each(this.request.headers, function iterator(k) {
    if (k === 'Host' || k === 'Content-Encoding' || k.match(/^X-Amz/i)) {
      headers.push(k);
    }
  });
  return headers;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.signature"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>signature (credentials)](#apidoc.element.vogels.AWS.Signers.V3.prototype.signature)
- description and source-code
```javascript
function signature(credentials) {
  return AWS.util.crypto.hmac(credentials.secretAccessKey, this.stringToSign(), 'base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.signedHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>signedHeaders ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.signedHeaders)
- description and source-code
```javascript
function signedHeaders() {
  var headers = [];
  AWS.util.arrayEach(this.headersToSign(), function iterator(h) {
    headers.push(h.toLowerCase());
  });
  return headers.sort().join(';');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.V3.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  var parts = [];
  parts.push(this.request.method);
  parts.push('/');
  parts.push('');
  parts.push(this.canonicalHeaders());
  parts.push(this.request.body);
  return AWS.util.crypto.sha256(parts.join('\n'));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.V3Https.prototype"></a>[module vogels.AWS.Signers.V3Https.prototype](#apidoc.module.vogels.AWS.Signers.V3Https.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.V3Https.prototype.authorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3Https.prototype.</span>authorization (credentials)](#apidoc.element.vogels.AWS.Signers.V3Https.prototype.authorization)
- description and source-code
```javascript
function authorization(credentials) {
  return 'AWS3-HTTPS ' +
    'AWSAccessKeyId=' + credentials.accessKeyId + ',' +
    'Algorithm=HmacSHA256,' +
    'Signature=' + this.signature(credentials);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3Https.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3Https.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Signers.V3Https.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V3Https.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V3Https.prototype.</span>stringToSign ()](#apidoc.element.vogels.AWS.Signers.V3Https.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign() {
  return this.request.headers['X-Amz-Date'];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Signers.V4.prototype"></a>[module vogels.AWS.Signers.V4.prototype](#apidoc.module.vogels.AWS.Signers.V4.prototype)

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.addAuthorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>addAuthorization (credentials, date)](#apidoc.element.vogels.AWS.Signers.V4.prototype.addAuthorization)
- description and source-code
```javascript
function addAuthorization(credentials, date) {
  var datetime = AWS.util.date.iso8601(date).replace(/[:\-]|\.\d{3}/g, '');

  if (this.isPresigned()) {
    this.updateForPresigned(credentials, datetime);
  } else {
    this.addHeaders(credentials, datetime);
  }

  this.request.headers['Authorization'] =
    this.authorization(credentials, datetime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.addHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>addHeaders (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.addHeaders)
- description and source-code
```javascript
function addHeaders(credentials, datetime) {
  this.request.headers['X-Amz-Date'] = datetime;
  if (credentials.sessionToken) {
    this.request.headers['x-amz-security-token'] = credentials.sessionToken;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.authorization"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>authorization (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.authorization)
- description and source-code
```javascript
function authorization(credentials, datetime) {
  var parts = [];
  var credString = this.credentialString(datetime);
  parts.push(this.algorithm + ' Credential=' +
    credentials.accessKeyId + '/' + credString);
  parts.push('SignedHeaders=' + this.signedHeaders());
  parts.push('Signature=' + this.signature(credentials, datetime));
  return parts.join(', ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalHeaderValues"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>canonicalHeaderValues (values)](#apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalHeaderValues)
- description and source-code
```javascript
function canonicalHeaderValues(values) {
  return values.replace(/\s+/g, ' ').replace(/^\s+|\s+$/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>canonicalHeaders ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalHeaders)
- description and source-code
```javascript
function canonicalHeaders() {
  var headers = [];
  AWS.util.each.call(this, this.request.headers, function (key, item) {
    headers.push([key, item]);
  });
  headers.sort(function (a, b) {
    return a[0].toLowerCase() < b[0].toLowerCase() ? -1 : 1;
  });
  var parts = [];
  AWS.util.arrayEach.call(this, headers, function (item) {
    var key = item[0].toLowerCase();
    if (this.isSignableHeader(key)) {
      parts.push(key + ':' +
        this.canonicalHeaderValues(item[1].toString()));
    }
  });
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalString"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>canonicalString ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.canonicalString)
- description and source-code
```javascript
function canonicalString() {
  var parts = [], pathname = this.request.pathname();
  if (this.serviceName !== 's3') pathname = AWS.util.uriEscapePath(pathname);

  parts.push(this.request.method);
  parts.push(pathname);
  parts.push(this.request.search());
  parts.push(this.canonicalHeaders() + '\n');
  parts.push(this.signedHeaders());
  parts.push(this.hexEncodedBodyHash());
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>constructor (request, serviceName, signatureCache)](#apidoc.element.vogels.AWS.Signers.V4.prototype.constructor)
- description and source-code
```javascript
function V4(request, serviceName, signatureCache) {
  AWS.Signers.RequestSigner.call(this, request);
  this.serviceName = serviceName;
  this.signatureCache = signatureCache;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.credentialString"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>credentialString (datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.credentialString)
- description and source-code
```javascript
function credentialString(datetime) {
  var parts = [];
  parts.push(datetime.substr(0, 8));
  parts.push(this.request.region);
  parts.push(this.serviceName);
  parts.push('aws4_request');
  return parts.join('/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.hexEncodedBodyHash"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>hexEncodedBodyHash ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.hexEncodedBodyHash)
- description and source-code
```javascript
function hexEncodedBodyHash() {
  if (this.isPresigned() && this.serviceName === 's3') {
    return 'UNSIGNED-PAYLOAD';
  } else if (this.request.headers['X-Amz-Content-Sha256']) {
    return this.request.headers['X-Amz-Content-Sha256'];
  } else {
    return this.hexEncodedHash(this.request.body || '');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.hexEncodedHash"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>hexEncodedHash (string)](#apidoc.element.vogels.AWS.Signers.V4.prototype.hexEncodedHash)
- description and source-code
```javascript
function hash(string) {
  return AWS.util.crypto.sha256(string, 'hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.isPresigned"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>isPresigned ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.isPresigned)
- description and source-code
```javascript
function isPresigned() {
  return this.request.headers[expiresHeader] ? true : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.isSignableHeader"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>isSignableHeader (key)](#apidoc.element.vogels.AWS.Signers.V4.prototype.isSignableHeader)
- description and source-code
```javascript
function isSignableHeader(key) {
  if (key.toLowerCase().indexOf('x-amz-') === 0) return true;
  return this.unsignableHeaders.indexOf(key) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.signature"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>signature (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.signature)
- description and source-code
```javascript
function signature(credentials, datetime) {
  var cache = null;
  if (this.signatureCache) {
    var cache = cachedSecret[this.serviceName];
  }
  var date = datetime.substr(0, 8);

  if (!cache ||
      cache.akid !== credentials.accessKeyId ||
      cache.region !== this.request.region ||
      cache.date !== date) {

    var kSecret = credentials.secretAccessKey;
    var kDate = AWS.util.crypto.hmac('AWS4' + kSecret, date, 'buffer');
    var kRegion = AWS.util.crypto.hmac(kDate, this.request.region, 'buffer');
    var kService = AWS.util.crypto.hmac(kRegion, this.serviceName, 'buffer');
    var kCredentials = AWS.util.crypto.hmac(kService, 'aws4_request', 'buffer');

    if (!this.signatureCache) {
      return AWS.util.crypto.hmac(kCredentials, this.stringToSign(datetime), 'hex');
    }

    cachedSecret[this.serviceName] = {
      region: this.request.region, date: date,
      key: kCredentials, akid: credentials.accessKeyId
    };
  }

  var key = cachedSecret[this.serviceName].key;
  return AWS.util.crypto.hmac(key, this.stringToSign(datetime), 'hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.signedHeaders"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>signedHeaders ()](#apidoc.element.vogels.AWS.Signers.V4.prototype.signedHeaders)
- description and source-code
```javascript
function signedHeaders() {
  var keys = [];
  AWS.util.each.call(this, this.request.headers, function (key) {
    key = key.toLowerCase();
    if (this.isSignableHeader(key)) keys.push(key);
  });
  return keys.sort().join(';');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>stringToSign (datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.stringToSign)
- description and source-code
```javascript
function stringToSign(datetime) {
  var parts = [];
  parts.push('AWS4-HMAC-SHA256');
  parts.push(datetime);
  parts.push(this.credentialString(datetime));
  parts.push(this.hexEncodedHash(this.canonicalString()));
  return parts.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Signers.V4.prototype.updateForPresigned"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Signers.V4.prototype.</span>updateForPresigned (credentials, datetime)](#apidoc.element.vogels.AWS.Signers.V4.prototype.updateForPresigned)
- description and source-code
```javascript
function updateForPresigned(credentials, datetime) {
  var credString = this.credentialString(datetime);
  var qs = {
    'X-Amz-Date': datetime,
    'X-Amz-Algorithm': this.algorithm,
    'X-Amz-Credential': credentials.accessKeyId + '/' + credString,
    'X-Amz-Expires': this.request.headers[expiresHeader],
    'X-Amz-SignedHeaders': this.signedHeaders()
  };

  if (credentials.sessionToken) {
    qs['X-Amz-Security-Token'] = credentials.sessionToken;
  }

  if (this.request.headers['Content-Type']) {
    qs['Content-Type'] = this.request.headers['Content-Type'];
  }
  if (this.request.headers['Content-MD5']) {
    qs['Content-MD5'] = this.request.headers['Content-MD5'];
  }
  if (this.request.headers['Cache-Control']) {
    qs['Cache-Control'] = this.request.headers['Cache-Control'];
  }

  // need to pull in any other X-Amz-* headers
  AWS.util.each.call(this, this.request.headers, function(key, value) {
    if (key === expiresHeader) return;
    if (this.isSignableHeader(key) &&
        key.toLowerCase().indexOf('x-amz-') === 0) {
      qs[key] = value;
    }
  });

  var sep = this.request.path.indexOf('?') >= 0 ? '&' : '?';
  this.request.path += sep + AWS.util.queryParamsToString(qs);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SimpleDB"></a>[module vogels.AWS.SimpleDB](#apidoc.module.vogels.AWS.SimpleDB)

#### <a name="apidoc.element.vogels.AWS.SimpleDB.SimpleDB"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>SimpleDB ()](#apidoc.element.vogels.AWS.SimpleDB.SimpleDB)
- description and source-code
```javascript
SimpleDB = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.SimpleDB.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.</span>__super__ (config)](#apidoc.element.vogels.AWS.SimpleDB.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.SimpleDB.prototype"></a>[module vogels.AWS.SimpleDB.prototype](#apidoc.module.vogels.AWS.SimpleDB.prototype)

#### <a name="apidoc.element.vogels.AWS.SimpleDB.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.SimpleDB.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.SimpleDB.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.StorageGateway"></a>[module vogels.AWS.StorageGateway](#apidoc.module.vogels.AWS.StorageGateway)

#### <a name="apidoc.element.vogels.AWS.StorageGateway.StorageGateway"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>StorageGateway ()](#apidoc.element.vogels.AWS.StorageGateway.StorageGateway)
- description and source-code
```javascript
StorageGateway = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.StorageGateway.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.</span>__super__ (config)](#apidoc.element.vogels.AWS.StorageGateway.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.StorageGateway.prototype"></a>[module vogels.AWS.StorageGateway.prototype](#apidoc.module.vogels.AWS.StorageGateway.prototype)

#### <a name="apidoc.element.vogels.AWS.StorageGateway.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.StorageGateway.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.StorageGateway.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Support"></a>[module vogels.AWS.Support](#apidoc.module.vogels.AWS.Support)

#### <a name="apidoc.element.vogels.AWS.Support.Support"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>Support ()](#apidoc.element.vogels.AWS.Support.Support)
- description and source-code
```javascript
Support = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.Support.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Support.</span>__super__ (config)](#apidoc.element.vogels.AWS.Support.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.Support.prototype"></a>[module vogels.AWS.Support.prototype](#apidoc.module.vogels.AWS.Support.prototype)

#### <a name="apidoc.element.vogels.AWS.Support.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.Support.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.Support.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.TemporaryCredentials"></a>[module vogels.AWS.TemporaryCredentials](#apidoc.module.vogels.AWS.TemporaryCredentials)

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials.TemporaryCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>TemporaryCredentials (params)](#apidoc.element.vogels.AWS.TemporaryCredentials.TemporaryCredentials)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.TemporaryCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.TemporaryCredentials.prototype"></a>[module vogels.AWS.TemporaryCredentials.prototype](#apidoc.module.vogels.AWS.TemporaryCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.constructor)
- description and source-code
```javascript
function TemporaryCredentials(params) {
  AWS.Credentials.call(this);
  this.loadMasterCredentials();
  this.expired = true;

  this.params = params || {};
  if (this.params.RoleArn) {
    this.params.RoleSessionName =
      this.params.RoleSessionName || 'temporary-credentials';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials.prototype.createClients"></a>[function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.createClients)
- description and source-code
```javascript
createClients = function () {
  this.service = this.service || new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials.prototype.loadMasterCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>loadMasterCredentials ()](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.loadMasterCredentials)
- description and source-code
```javascript
function loadMasterCredentials() {
  this.masterCredentials = AWS.config.credentials;
  while (this.masterCredentials.masterCredentials) {
    this.masterCredentials = this.masterCredentials.masterCredentials;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.TemporaryCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.TemporaryCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.TemporaryCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  self.createClients();
  if (!callback) callback = function(err) { if (err) throw err; };

  self.service.config.credentials = self.masterCredentials;
  var operation = self.params.RoleArn ?
    self.service.assumeRole : self.service.getSessionToken;
  operation.call(self.service, function (err, data) {
    if (!err) {
      self.service.credentialsFrom(data, self);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.WAF"></a>[module vogels.AWS.WAF](#apidoc.module.vogels.AWS.WAF)

#### <a name="apidoc.element.vogels.AWS.WAF.WAF"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>WAF ()](#apidoc.element.vogels.AWS.WAF.WAF)
- description and source-code
```javascript
WAF = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WAF.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WAF.</span>__super__ (config)](#apidoc.element.vogels.AWS.WAF.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.WAF.prototype"></a>[module vogels.AWS.WAF.prototype](#apidoc.module.vogels.AWS.WAF.prototype)

#### <a name="apidoc.element.vogels.AWS.WAF.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WAF.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.WAF.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.WebIdentityCredentials"></a>[module vogels.AWS.WebIdentityCredentials](#apidoc.module.vogels.AWS.WebIdentityCredentials)

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials.WebIdentityCredentials"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>WebIdentityCredentials (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials.WebIdentityCredentials)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.</span>__super__ ()](#apidoc.element.vogels.AWS.WebIdentityCredentials.__super__)
- description and source-code
```javascript
function Credentials() {
  // hide secretAccessKey from being displayed with util.inspect
  AWS.util.hideProperties(this, ['secretAccessKey']);

  this.expired = false;
  this.expireTime = null;
  if (arguments.length === 1 && typeof arguments[0] === 'object') {
    var creds = arguments[0].credentials || arguments[0];
    this.accessKeyId = creds.accessKeyId;
    this.secretAccessKey = creds.secretAccessKey;
    this.sessionToken = creds.sessionToken;
  } else {
    this.accessKeyId = arguments[0];
    this.secretAccessKey = arguments[1];
    this.sessionToken = arguments[2];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.WebIdentityCredentials.prototype"></a>[module vogels.AWS.WebIdentityCredentials.prototype](#apidoc.module.vogels.AWS.WebIdentityCredentials.prototype)

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.prototype.</span>constructor (params)](#apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.constructor)
- description and source-code
```javascript
function WebIdentityCredentials(params) {
  AWS.Credentials.call(this);
  this.expired = true;
  this.params = params;
  this.params.RoleSessionName = this.params.RoleSessionName || 'web-identity';
  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.createClients"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.prototype.</span>createClients ()](#apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.createClients)
- description and source-code
```javascript
createClients = function () {
  this.service = this.service || new AWS.STS({params: this.params});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.refresh"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WebIdentityCredentials.prototype.</span>refresh (callback)](#apidoc.element.vogels.AWS.WebIdentityCredentials.prototype.refresh)
- description and source-code
```javascript
function refresh(callback) {
  var self = this;
  self.createClients();
  if (!callback) callback = function(err) { if (err) throw err; };

  self.service.assumeRoleWithWebIdentity(function (err, data) {
    self.data = null;
    if (!err) {
      self.data = data;
      self.service.credentialsFrom(data, self);
    }
    callback(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.WorkSpaces"></a>[module vogels.AWS.WorkSpaces](#apidoc.module.vogels.AWS.WorkSpaces)

#### <a name="apidoc.element.vogels.AWS.WorkSpaces.WorkSpaces"></a>[function <span class="apidocSignatureSpan">vogels.AWS.</span>WorkSpaces ()](#apidoc.element.vogels.AWS.WorkSpaces.WorkSpaces)
- description and source-code
```javascript
WorkSpaces = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.WorkSpaces.__super__"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.</span>__super__ (config)](#apidoc.element.vogels.AWS.WorkSpaces.__super__)
- description and source-code
```javascript
function Service(config) {
  if (!this.loadServiceClass) {
    throw AWS.util.error(new Error(),
      'Service must be constructed with 'new\' operator');
  }
  var ServiceClass = this.loadServiceClass(config || {});
  if (ServiceClass) return new ServiceClass(config);
  this.initialize(config);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.WorkSpaces.prototype"></a>[module vogels.AWS.WorkSpaces.prototype](#apidoc.module.vogels.AWS.WorkSpaces.prototype)

#### <a name="apidoc.element.vogels.AWS.WorkSpaces.prototype.constructor"></a>[function <span class="apidocSignatureSpan">vogels.AWS.WorkSpaces.prototype.</span>constructor ()](#apidoc.element.vogels.AWS.WorkSpaces.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  if (klass !== Object) {
    return klass.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.XML"></a>[module vogels.AWS.XML](#apidoc.module.vogels.AWS.XML)

#### <a name="apidoc.element.vogels.AWS.XML.Builder"></a>[function <span class="apidocSignatureSpan">vogels.AWS.XML.</span>Builder ()](#apidoc.element.vogels.AWS.XML.Builder)
- description and source-code
```javascript
function XmlBuilder() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.XML.Parser"></a>[function <span class="apidocSignatureSpan">vogels.AWS.XML.</span>Parser ()](#apidoc.element.vogels.AWS.XML.Parser)
- description and source-code
```javascript
function NodeXmlParser() { }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.XML.Builder.prototype"></a>[module vogels.AWS.XML.Builder.prototype](#apidoc.module.vogels.AWS.XML.Builder.prototype)

#### <a name="apidoc.element.vogels.AWS.XML.Builder.prototype.toXML"></a>[function <span class="apidocSignatureSpan">vogels.AWS.XML.Builder.prototype.</span>toXML (params, shape, rootElement, noEmpty)](#apidoc.element.vogels.AWS.XML.Builder.prototype.toXML)
- description and source-code
```javascript
toXML = function (params, shape, rootElement, noEmpty) {
  var xml = builder.create(rootElement);
  applyNamespaces(xml, shape);
  serialize(xml, params, shape);
  return xml.children.length > 0 || noEmpty ? xml.root().toString() : '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.XML.Parser.prototype"></a>[module vogels.AWS.XML.Parser.prototype](#apidoc.module.vogels.AWS.XML.Parser.prototype)

#### <a name="apidoc.element.vogels.AWS.XML.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.XML.Parser.prototype.</span>parse (xml, shape)](#apidoc.element.vogels.AWS.XML.Parser.prototype.parse)
- description and source-code
```javascript
parse = function (xml, shape) {
  shape = shape || {};

  var result = null;
  var error = null;

  var parser = new xml2js.Parser(options);
  parser.parseString(xml, function (e, r) {
    error = e;
    result = r;
  });

  if (result) {
    var data = parseXml(result, shape);
    if (result.ResponseMetadata) {
      data.ResponseMetadata = parseXml(result.ResponseMetadata[0], {});
    }
    return data;
  } else if (error) {
    throw util.error(error, {code: 'XMLParserError', retryable: true});
  } else { // empty xml document
    return parseXml({}, shape);
  }
}
```
- example usage
```shell
...
  });
};

internals.updateExpressions = function (schema, data, options) {
  var exp = expressions.serializeUpdateExpression(schema, data);

  if(options.UpdateExpression) {
    var parsed = expressions.parse(options.UpdateExpression);

    exp.expressions = _.reduce(parsed, function (result, val, key) {
if(!_.isEmpty(val)) {
  result[key] = result[key].concat(val);
}

return result;
...
```



# <a name="apidoc.module.vogels.AWS.util"></a>[module vogels.AWS.util](#apidoc.module.vogels.AWS.util)

#### <a name="apidoc.element.vogels.AWS.util.Buffer"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.vogels.AWS.util.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
...
    var len = value.length;
    var bin = new Uint8Array(new ArrayBuffer(len));
    for (var i = 0; i < len; i++) {
      bin[i] = value.charCodeAt(i);
    }
    return bin;
  } else {
    return AWS.util.Buffer(value);
  }
};
...
```

#### <a name="apidoc.element.vogels.AWS.util.applyClockOffset"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>applyClockOffset (serverTime)](#apidoc.element.vogels.AWS.util.applyClockOffset)
- description and source-code
```javascript
function applyClockOffset(serverTime) {
  if (serverTime)
    AWS.config.systemClockOffset = serverTime - new Date().getTime();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.arrayEach"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>arrayEach (array, iterFunction)](#apidoc.element.vogels.AWS.util.arrayEach)
- description and source-code
```javascript
function arrayEach(array, iterFunction) {
  for (var idx in array) {
    if (array.hasOwnProperty(idx)) {
      var ret = iterFunction.call(this, array[idx], parseInt(idx, 10));
      if (ret === util.abort) break;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.arraySliceFn"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>arraySliceFn (obj)](#apidoc.element.vogels.AWS.util.arraySliceFn)
- description and source-code
```javascript
function arraySliceFn(obj) {
  var fn = obj.slice || obj.webkitSlice || obj.mozSlice;
  return typeof fn === 'function' ? fn : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.computeSha256"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>computeSha256 (body, done)](#apidoc.element.vogels.AWS.util.computeSha256)
- description and source-code
```javascript
function computeSha256(body, done) {
  if (util.isNode()) {
    var Stream = util.nodeRequire('stream').Stream;
    var fs = util.nodeRequire('fs');
    if (body instanceof Stream) {
      if (typeof body.path === 'string') { // assume file object
        body = fs.createReadStream(body.path);
      } else { // TODO support other stream types
        return done(new Error('Non-file stream objects are ' +
                              'not supported with SigV4'));
      }
    }
  }

  util.crypto.sha256(body, 'hex', function(err, sha) {
    if (err) done(err);
    else done(null, sha);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.copy"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>copy (object)](#apidoc.element.vogels.AWS.util.copy)
- description and source-code
```javascript
function copy(object) {
  if (object === null || object === undefined) return object;
  var dupe = {};
  // jshint forin:false
  for (var key in object) {
    dupe[key] = object[key];
  }
  return dupe;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.each"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>each (object, iterFunction)](#apidoc.element.vogels.AWS.util.each)
- description and source-code
```javascript
function each(object, iterFunction) {
  for (var key in object) {
    if (Object.prototype.hasOwnProperty.call(object, key)) {
      var ret = iterFunction.call(this, key, object[key]);
      if (ret === util.abort) break;
    }
  }
}
```
- example usage
```shell
...

  if(_.isPlainObject(hashKey)) {
    obj[schema.hashKey] = hashKey[schema.hashKey];

    if(schema.rangeKey && !_.isNull(hashKey[schema.rangeKey]) && !_.isUndefined(hashKey[schema.rangeKey])) {
obj[schema.rangeKey] = hashKey[schema.rangeKey];
    }
    _.each(schema.globalIndexes, function (keys) {
if(_.has(hashKey, keys.hashKey)){
  obj[keys.hashKey] = hashKey[keys.hashKey];
}

if(_.has(hashKey, keys.rangeKey)){
  obj[keys.rangeKey] = hashKey[keys.rangeKey];
}
...
```

#### <a name="apidoc.element.vogels.AWS.util.engine"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>engine ()](#apidoc.element.vogels.AWS.util.engine)
- description and source-code
```javascript
function engine() {
  if (util.isBrowser() && typeof navigator !== 'undefined') {
    return navigator.userAgent;
  } else {
    return process.platform + '/' + process.version;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.error"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>error (err, options)](#apidoc.element.vogels.AWS.util.error)
- description and source-code
```javascript
function error(err, options) {
  var originalError = null;
  if (typeof err.message === 'string' && err.message !== '') {
    if (typeof options === 'string' || (options && options.message)) {
      originalError = util.copy(err);
      originalError.message = err.message;
    }
  }
  err.message = err.message || null;

  if (typeof options === 'string') {
    err.message = options;
  } else if (typeof options === 'object' && options !== null) {
    util.update(err, options);
    if (options.message)
      err.message = options.message;
    if (options.code || options.name)
      err.code = options.code || options.name;
    if (options.stack)
      err.stack = options.stack;
  }

  if (typeof Object.defineProperty === 'function') {
    Object.defineProperty(err, 'name', {writable: true, enumerable: false});
    Object.defineProperty(err, 'message', {enumerable: true});
  }

  err.name = options && options.name || err.name || err.code || 'Error';
  err.time = new Date();

  if (originalError) err.originalError = originalError;

  return err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.extractRequestId"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>extractRequestId (resp)](#apidoc.element.vogels.AWS.util.extractRequestId)
- description and source-code
```javascript
function extractRequestId(resp) {
  var requestId = resp.httpResponse.headers['x-amz-request-id'] ||
                   resp.httpResponse.headers['x-amzn-requestid'];

  if (!requestId && resp.data && resp.data.ResponseMetadata) {
    requestId = resp.data.ResponseMetadata.RequestId;
  }

  if (requestId) {
    resp.requestId = requestId;
  }

  if (resp.error) {
    resp.error.requestId = requestId;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.hideProperties"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>hideProperties (obj, props)](#apidoc.element.vogels.AWS.util.hideProperties)
- description and source-code
```javascript
function hideProperties(obj, props) {
  if (typeof Object.defineProperty !== 'function') return;

  util.arrayEach(props, function (key) {
    Object.defineProperty(obj, key, {
      enumerable: false, writable: true, configurable: true });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.hoistPayloadMember"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>hoistPayloadMember (resp)](#apidoc.element.vogels.AWS.util.hoistPayloadMember)
- description and source-code
```javascript
function hoistPayloadMember(resp) {
  var req = resp.request;
  var operation = req.operation;
  var output = req.service.api.operations[operation].output;
  if (output.payload) {
    var payloadMember = output.members[output.payload];
    var responsePayload = resp.data[output.payload];
    if (payloadMember.type === 'structure') {
      util.each(responsePayload, function(key, value) {
        util.property(resp.data, key, value, false);
      });
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.inherit"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>inherit (klass, features)](#apidoc.element.vogels.AWS.util.inherit)
- description and source-code
```javascript
function inherit(klass, features) {
  var newObject = null;
  if (features === undefined) {
    features = klass;
    klass = Object;
    newObject = {};
  } else {
    var ctor = function ConstructorWrapper() {};
    ctor.prototype = klass.prototype;
    newObject = new ctor();
  }

  // constructor not supplied, create pass-through ctor
  if (features.constructor === Object) {
    features.constructor = function() {
      if (klass !== Object) {
        return klass.apply(this, arguments);
      }
    };
  }

  features.constructor.prototype = newObject;
  util.update(features.constructor.prototype, features);
  features.constructor.__super__ = klass;
  return features.constructor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.isBrowser"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isBrowser ()](#apidoc.element.vogels.AWS.util.isBrowser)
- description and source-code
```javascript
function isBrowser() { return process && process.browser; }
```
- example usage
```shell
...

utils.strToBin = function (value) {
if (typeof(value) !== 'string') {
  var StrConversionError = 'Need to pass in string primitive to be converted to binary.';
  throw new Error(StrConversionError);
}

if (AWS.util.isBrowser()) {
  var len = value.length;
  var bin = new Uint8Array(new ArrayBuffer(len));
  for (var i = 0; i < len; i++) {
    bin[i] = value.charCodeAt(i);
  }
  return bin;
} else {
...
```

#### <a name="apidoc.element.vogels.AWS.util.isClockSkewed"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isClockSkewed (serverTime)](#apidoc.element.vogels.AWS.util.isClockSkewed)
- description and source-code
```javascript
function isClockSkewed(serverTime) {
  if (serverTime) {
    util.property(AWS.config, 'isClockSkewed',
      Math.abs(new Date().getTime() - serverTime) >= 300000, false);
    return AWS.config.isClockSkewed;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.isEmpty"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isEmpty (obj)](#apidoc.element.vogels.AWS.util.isEmpty)
- description and source-code
```javascript
function isEmpty(obj) {
  for (var prop in obj) {
    if (obj.hasOwnProperty(prop)) {
      return false;
    }
  }
  return true;
}
```
- example usage
```shell
...
    responses.push(resp);

    return callback();
  });
};

var testFunc = function () {
  return request !== null && !_.isEmpty(request);
};

var resulsFunc = function (err) {
  if(err) {
    return callback(err);
  }
...
```

#### <a name="apidoc.element.vogels.AWS.util.isNode"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isNode ()](#apidoc.element.vogels.AWS.util.isNode)
- description and source-code
```javascript
function isNode() { return !util.isBrowser(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.isType"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>isType (obj, type)](#apidoc.element.vogels.AWS.util.isType)
- description and source-code
```javascript
function isType(obj, type) {
  // handle cross-"frame" objects
  if (typeof type === 'function') type = util.typeName(type);
  return Object.prototype.toString.call(obj) === '[object ' + type + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.memoizedProperty"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>memoizedProperty (obj, name, get, enumerable)](#apidoc.element.vogels.AWS.util.memoizedProperty)
- description and source-code
```javascript
function memoizedProperty(obj, name, get, enumerable) {
  var cachedValue = null;

  // build enumerable attribute for each value with lazy accessor.
  util.property(obj, name, function() {
    if (cachedValue === null) {
      cachedValue = get();
    }
    return cachedValue;
  }, enumerable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.merge"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>merge (obj1, obj2)](#apidoc.element.vogels.AWS.util.merge)
- description and source-code
```javascript
function merge(obj1, obj2) {
  return util.update(util.copy(obj1), obj2);
}
```
- example usage
```shell
...
  async = require('async');

var internals = {};

internals.buildInitialGetItemsRequest = function (tableName, keys, options) {
var request = {};

request[tableName] = _.merge({}, {Keys : keys}, options);

return { RequestItems : request };
};

internals.serializeKeys = function (keys, table, serializer) {
return keys.map(function (key) {
  return serializer.buildKey(key, null, table.schema);
...
```

#### <a name="apidoc.element.vogels.AWS.util.mixin"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>mixin ()](#apidoc.element.vogels.AWS.util.mixin)
- description and source-code
```javascript
function mixin() {
  var klass = arguments[0];
  for (var i = 1; i < arguments.length; i++) {
    // jshint forin:false
    for (var prop in arguments[i].prototype) {
      var fn = arguments[i].prototype[prop];
      if (prop !== 'constructor') {
        klass.prototype[prop] = fn;
      }
    }
  }
  return klass;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.multiRequire"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>multiRequire (module1, module2)](#apidoc.element.vogels.AWS.util.multiRequire)
- description and source-code
```javascript
function multiRequire(module1, module2) {
  return require(util.isNode() ? module1 : module2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.nodeRequire"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>nodeRequire (module)](#apidoc.element.vogels.AWS.util.nodeRequire)
- description and source-code
```javascript
function nodeRequire(module) {
  if (util.isNode()) return require(module);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.property"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>property (obj, name, value, enumerable, isValue)](#apidoc.element.vogels.AWS.util.property)
- description and source-code
```javascript
function property(obj, name, value, enumerable, isValue) {
  var opts = {
    configurable: true,
    enumerable: enumerable !== undefined ? enumerable : true
  };
  if (typeof value === 'function' && !isValue) {
    opts.get = value;
  }
  else {
    opts.value = value; opts.writable = true;
  }

  Object.defineProperty(obj, name, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.queryParamsToString"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>queryParamsToString (params)](#apidoc.element.vogels.AWS.util.queryParamsToString)
- description and source-code
```javascript
function queryParamsToString(params) {
  var items = [];
  var escape = util.uriEscape;
  var sortedKeys = Object.keys(params).sort();

  util.arrayEach(sortedKeys, function(name) {
    var value = params[name];
    var ename = escape(name);
    var result = ename + '=';
    if (Array.isArray(value)) {
      var vals = [];
      util.arrayEach(value, function(item) { vals.push(escape(item)); });
      result = ename + '=' + vals.sort().join('&' + ename + '=');
    } else if (value !== undefined && value !== null) {
      result = ename + '=' + escape(value);
    }
    items.push(result);
  });

  return items.join('&');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.queryStringParse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>queryStringParse (qs)](#apidoc.element.vogels.AWS.util.queryStringParse)
- description and source-code
```javascript
function queryStringParse(qs) {
  return require('querystring').parse(qs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.readFileSync"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>readFileSync (path)](#apidoc.element.vogels.AWS.util.readFileSync)
- description and source-code
```javascript
function readFileSync(path) {
  if (typeof window !== 'undefined') return null;
  return util.nodeRequire('fs').readFileSync(path, 'utf-8');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.typeName"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>typeName (type)](#apidoc.element.vogels.AWS.util.typeName)
- description and source-code
```javascript
function typeName(type) {
  if (type.hasOwnProperty('name')) return type.name;
  var str = type.toString();
  var match = str.match(/^\s*function (.+)\(/);
  return match ? match[1] : str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.update"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>update (obj1, obj2)](#apidoc.element.vogels.AWS.util.update)
- description and source-code
```javascript
function update(obj1, obj2) {
  util.each(obj2, function iterator(key, item) {
    obj1[key] = item;
  });
  return obj1;
}
```
- example usage
```shell
...
vogels.AWS.config.loadFromPath('credentials.json');
'''

When running on EC2 its recommended to leverage EC2 IAM roles. If you have configured your instance to use IAM roles, Vogels will
 automatically select these credentials for use in your application, and you do not need to manually provide credentials in any
other format.

'''js
var vogels = require('vogels');
vogels.AWS.config.update({region: "REGION"}); // region must be set
'''

You can also directly pass in your access key id, secret and region.
  * Its recommend you not hard-code credentials inside an application. Use this method only for small personal scripts or for testing
 purposes.

'''js
var vogels = require('vogels');
...
```

#### <a name="apidoc.element.vogels.AWS.util.uriEscape"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>uriEscape (string)](#apidoc.element.vogels.AWS.util.uriEscape)
- description and source-code
```javascript
function uriEscape(string) {
  var output = encodeURIComponent(string);
  output = output.replace(/[^A-Za-z0-9_.~\-%]+/g, escape);

  // AWS percent-encodes some extra non-standard characters in a URI
  output = output.replace(/[*]/g, function(ch) {
    return '%' + ch.charCodeAt(0).toString(16).toUpperCase();
  });

  return output;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.uriEscapePath"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>uriEscapePath (string)](#apidoc.element.vogels.AWS.util.uriEscapePath)
- description and source-code
```javascript
function uriEscapePath(string) {
  var parts = [];
  util.arrayEach(string.split('/'), function (part) {
    parts.push(util.uriEscape(part));
  });
  return parts.join('/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.urlFormat"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>urlFormat (url)](#apidoc.element.vogels.AWS.util.urlFormat)
- description and source-code
```javascript
function urlFormat(url) {
  return require('url').format(url);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.urlParse"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>urlParse (url)](#apidoc.element.vogels.AWS.util.urlParse)
- description and source-code
```javascript
function urlParse(url) {
  return require('url').parse(url);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.userAgent"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.</span>userAgent ()](#apidoc.element.vogels.AWS.util.userAgent)
- description and source-code
```javascript
function userAgent() {
  var name = util.isBrowser() ? 'js' : 'nodejs';
  var agent = 'aws-sdk-' + name + '/' + require('./core').VERSION;
  if (name === 'nodejs') agent += ' ' + util.engine();
  return agent;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.AWS.util.Buffer.prototype"></a>[module vogels.AWS.util.Buffer.prototype](#apidoc.module.vogels.AWS.util.Buffer.prototype)

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.asciiSlice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.asciiSlice)
- description and source-code
```javascript
function asciiSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.asciiWrite"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.asciiWrite)
- description and source-code
```javascript
function asciiWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.base64Slice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>base64Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.base64Slice)
- description and source-code
```javascript
function base64Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.base64Write"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>base64Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.base64Write)
- description and source-code
```javascript
function base64Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.compare"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.vogels.AWS.util.Buffer.prototype.compare)
- description and source-code
```javascript
function compare(target, start, end, thisStart, thisEnd) {

  if (!(target instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');
  if (arguments.length === 1)
    return compare_(this, target);

  if (start === undefined)
    start = 0;
  else if (start < 0)
    throw new RangeError('out of range index');
  else
    start >>>= 0;

  if (end === undefined)
    end = target.length;
  else if (end > target.length)
    throw new RangeError('out of range index');
  else
    end >>>= 0;

  if (thisStart === undefined)
    thisStart = 0;
  else if (thisStart < 0)
    throw new RangeError('out of range index');
  else
    thisStart >>>= 0;

  if (thisEnd === undefined)
    thisEnd = this.length;
  else if (thisEnd > this.length)
    throw new RangeError('out of range index');
  else
    thisEnd >>>= 0;

  if (thisStart >= thisEnd)
    return (start >= end ? 0 : -1);
  else if (start >= end)
    return 1;

  return compareOffset(this, target, start, thisStart, end, thisEnd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.copy"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>copy ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.copy)
- description and source-code
```javascript
function copy() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.equals"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>equals (b)](#apidoc.element.vogels.AWS.util.Buffer.prototype.equals)
- description and source-code
```javascript
function equals(b) {
  if (!(b instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');

  if (this === b)
    return true;

  return binding.compare(this, b) === 0;
}
```
- example usage
```shell
...

Vogels supports all the possible KeyConditions that DynamoDB currently
supports.

'''js
BlogPost
.query('werner@example.com')
.where('title').equals('Expanding')
.exec();

// less than equals
BlogPost
.query('werner@example.com')
.where('title').lte('Expanding')
.exec();
...
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.fill"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.fill)
- description and source-code
```javascript
function fill(val, start, end, encoding) {
  // Handle string cases:
  if (typeof val === 'string') {
    if (typeof start === 'string') {
      encoding = start;
      start = 0;
      end = this.length;
    } else if (typeof end === 'string') {
      encoding = end;
      end = this.length;
    }

    if (encoding !== undefined && typeof encoding !== 'string') {
      throw new TypeError('encoding must be a string');
    }
    var normalizedEncoding = internalUtil.normalizeEncoding(encoding);
    if (normalizedEncoding === undefined) {
      throw new TypeError('Unknown encoding: ' + encoding);
    }

    if (val.length === 0) {
      // Previously, if val === '', the Buffer would not fill,
      // which is rather surprising.
      val = 0;
    } else if (val.length === 1) {
      var code = val.charCodeAt(0);
      if ((normalizedEncoding === 'utf8' && code < 128) ||
          normalizedEncoding === 'latin1') {
        // Fast path: If 'val' fits into a single byte, use that numeric value.
        val = code;
      }
    }
  } else if (typeof val === 'number') {
    val = val & 255;
  }

  // Invalid ranges are not set to a default, so can range check early.
  if (start < 0 || end > this.length)
    throw new RangeError('Out of range index');

  if (end <= start)
    return this;

  start = start >>> 0;
  end = end === undefined ? this.length : end >>> 0;

  binding.fill(this, val, start, end, encoding);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.hexSlice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>hexSlice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.hexSlice)
- description and source-code
```javascript
function hexSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.hexWrite"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>hexWrite ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.hexWrite)
- description and source-code
```javascript
function hexWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.includes"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.includes)
- description and source-code
```javascript
function includes(val, byteOffset, encoding) {
  return this.indexOf(val, byteOffset, encoding) !== -1;
}
```
- example usage
```shell
...
    return val.toISOString();
  }

  return val;
};

internals.isFunctionOperator = function (operator) {
  return _.includes(['attribute_exists',
                     'attribute_not_exists',
                     'attribute_type',
                     'begins_with',
                     'contains',
                     'NOT contains',
                     'size'], operator);
};
...
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.indexOf)
- description and source-code
```javascript
function indexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.inspect"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>inspect ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.inspect)
- description and source-code
```javascript
function inspect() {
  var str = '';
  var max = exports.INSPECT_MAX_BYTES;
  if (this.length > 0) {
    str = this.toString('hex', 0, max).match(/.{2}/g).join(' ');
    if (this.length > max)
      str += ' ... ';
  }
  return '<' + this.constructor.name + ' ' + str + '>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.latin1Slice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.latin1Slice)
- description and source-code
```javascript
function latin1Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.latin1Write"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>latin1Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.latin1Write)
- description and source-code
```javascript
function latin1Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readDoubleBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readDoubleBE)
- description and source-code
```javascript
function readDoubleBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readDoubleLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readDoubleLE)
- description and source-code
```javascript
function readDoubleLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readFloatBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readFloatBE)
- description and source-code
```javascript
function readFloatBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readFloatLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readFloatLE)
- description and source-code
```javascript
function readFloatLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readInt16BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt16BE)
- description and source-code
```javascript
readInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset + 1] | (this[offset] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readInt16LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt16LE)
- description and source-code
```javascript
readInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset] | (this[offset + 1] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readInt32BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt32BE)
- description and source-code
```javascript
readInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] << 24) |
      (this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      (this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readInt32LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt32LE)
- description and source-code
```javascript
readInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16) |
      (this[offset + 3] << 24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readInt8"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readInt8)
- description and source-code
```javascript
readInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  var val = this[offset];
  return !(val & 0x80) ? val : (0xff - val + 1) * -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readIntBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readIntBE)
- description and source-code
```javascript
readIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var i = byteLength;
  var mul = 1;
  var val = this[offset + --i];
  while (i > 0 && (mul *= 0x100))
    val += this[offset + --i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readIntLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readIntLE)
- description and source-code
```javascript
readIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt16BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt16BE)
- description and source-code
```javascript
readUInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return (this[offset] << 8) | this[offset + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt16LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt16LE)
- description and source-code
```javascript
readUInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return this[offset] | (this[offset + 1] << 8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt32BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt32BE)
- description and source-code
```javascript
readUInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] * 0x1000000) +
      ((this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt32LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt32LE)
- description and source-code
```javascript
readUInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return ((this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16)) +
      (this[offset + 3] * 0x1000000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt8"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUInt8)
- description and source-code
```javascript
readUInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  return this[offset];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUIntBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUIntBE)
- description and source-code
```javascript
readUIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset + --byteLength];
  var mul = 1;
  while (byteLength > 0 && (mul *= 0x100))
    val += this[offset + --byteLength] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.readUIntLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.readUIntLE)
- description and source-code
```javascript
readUIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.slice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>slice (start, end)](#apidoc.element.vogels.AWS.util.Buffer.prototype.slice)
- description and source-code
```javascript
function slice(start, end) {
  const srcLength = this.length;
  start = adjustOffset(start, srcLength);
  end = end !== undefined ? adjustOffset(end, srcLength) : srcLength;
  const newLength = end > start ? end - start : 0;
  return new FastBuffer(this.buffer, this.byteOffset + start, newLength);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.swap16"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>swap16 ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.swap16)
- description and source-code
```javascript
function swap16() {
  // For Buffer.length < 128, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 2 !== 0)
    throw new RangeError('Buffer size must be a multiple of 16-bits');
  if (len < 128) {
    for (var i = 0; i < len; i += 2)
      swap(this, i, i + 1);
    return this;
  }
  return swap16n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.swap32"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>swap32 ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.swap32)
- description and source-code
```javascript
function swap32() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 4 !== 0)
    throw new RangeError('Buffer size must be a multiple of 32-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 4) {
      swap(this, i, i + 3);
      swap(this, i + 1, i + 2);
    }
    return this;
  }
  return swap32n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.swap64"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>swap64 ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.swap64)
- description and source-code
```javascript
function swap64() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 8 !== 0)
    throw new RangeError('Buffer size must be a multiple of 64-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 8) {
      swap(this, i, i + 7);
      swap(this, i + 1, i + 6);
      swap(this, i + 2, i + 5);
      swap(this, i + 3, i + 4);
    }
    return this;
  }
  return swap64n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>toJSON ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this.length) {
    const data = [];
    for (var i = 0; i < this.length; ++i)
      data[i] = this[i];
    return { type: 'Buffer', data };
  } else {
    return { type: 'Buffer', data: [] };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.toString"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>toString ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.toString)
- description and source-code
```javascript
toString = function () {
  let result;
  if (arguments.length === 0) {
    result = this.utf8Slice(0, this.length);
  } else {
    result = slowToString.apply(this, arguments);
  }
  if (result === undefined)
    throw new Error('"toString()" failed');
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.ucs2Slice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.ucs2Slice)
- description and source-code
```javascript
function ucs2Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.ucs2Write"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.ucs2Write)
- description and source-code
```javascript
function ucs2Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.utf8Slice"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.utf8Slice)
- description and source-code
```javascript
function utf8Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.utf8Write"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>utf8Write ()](#apidoc.element.vogels.AWS.util.Buffer.prototype.utf8Write)
- description and source-code
```javascript
function utf8Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.write"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.vogels.AWS.util.Buffer.prototype.write)
- description and source-code
```javascript
write = function (string, offset, length, encoding) {
  // Buffer#write(string);
  if (offset === undefined) {
    encoding = 'utf8';
    length = this.length;
    offset = 0;

  // Buffer#write(string, encoding)
  } else if (length === undefined && typeof offset === 'string') {
    encoding = offset;
    length = this.length;
    offset = 0;

  // Buffer#write(string, offset[, length][, encoding])
  } else if (isFinite(offset)) {
    offset = offset >>> 0;
    if (isFinite(length)) {
      length = length >>> 0;
      if (encoding === undefined)
        encoding = 'utf8';
    } else {
      encoding = length;
      length = undefined;
    }
  } else {
    // if someone is still calling the obsolete form of write(), tell them.
    // we don't want eg buf.write("foo", "utf8", 10) to silently turn into
    // buf.write("foo", "utf8"), so we can't ignore extra args
    throw new Error('Buffer.write(string, encoding, offset[, length]) ' +
                    'is no longer supported');
  }

  var remaining = this.length - offset;
  if (length === undefined || length > remaining)
    length = remaining;

  if (string.length > 0 && (length < 0 || offset < 0))
    throw new RangeError('Attempt to write outside buffer bounds');

  if (!encoding)
    encoding = 'utf8';

  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'hex':
        return this.hexWrite(string, offset, length);

      case 'utf8':
      case 'utf-8':
        return this.utf8Write(string, offset, length);

      case 'ascii':
        return this.asciiWrite(string, offset, length);

      case 'latin1':
      case 'binary':
        return this.latin1Write(string, offset, length);

      case 'base64':
        // Warning: maxLength not taken into account in base64Write
        return this.base64Write(string, offset, length);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return this.ucs2Write(string, offset, length);

      default:
        if (loweredCase)
          throw new TypeError('Unknown encoding: ' + encoding);
        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeDoubleBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeDoubleBE)
- description and source-code
```javascript
function writeDoubleBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleBE(this, val, offset);
  else
    binding.writeDoubleBE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeDoubleLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeDoubleLE)
- description and source-code
```javascript
function writeDoubleLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleLE(this, val, offset);
  else
    binding.writeDoubleLE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeFloatBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeFloatBE)
- description and source-code
```javascript
function writeFloatBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatBE(this, val, offset);
  else
    binding.writeFloatBE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeFloatLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeFloatLE)
- description and source-code
```javascript
function writeFloatLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatLE(this, val, offset);
  else
    binding.writeFloatLE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt16BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt16BE)
- description and source-code
```javascript
writeInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt16LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt16LE)
- description and source-code
```javascript
writeInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt32BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt32BE)
- description and source-code
```javascript
writeInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt32LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt32LE)
- description and source-code
```javascript
writeInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  this[offset + 2] = (value >>> 16);
  this[offset + 3] = (value >>> 24);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt8"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeInt8)
- description and source-code
```javascript
writeInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0x7f, -0x80);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeIntBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeIntBE)
- description and source-code
```javascript
writeIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = byteLength - 1;
  var mul = 1;
  var sub = 0;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i + 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeIntLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeIntLE)
- description and source-code
```javascript
writeIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = 0;
  var mul = 1;
  var sub = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i - 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt16BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt16BE)
- description and source-code
```javascript
writeUInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt16LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt16LE)
- description and source-code
```javascript
writeUInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt32BE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt32BE)
- description and source-code
```javascript
writeUInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt32LE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt32LE)
- description and source-code
```javascript
writeUInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset + 3] = (value >>> 24);
  this[offset + 2] = (value >>> 16);
  this[offset + 1] = (value >>> 8);
  this[offset] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt8"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUInt8)
- description and source-code
```javascript
writeUInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0xff, 0);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUIntBE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUIntBE)
- description and source-code
```javascript
writeUIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var i = byteLength - 1;
  var mul = 1;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.AWS.util.Buffer.prototype.writeUIntLE"></a>[function <span class="apidocSignatureSpan">vogels.AWS.util.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.vogels.AWS.util.Buffer.prototype.writeUIntLE)
- description and source-code
```javascript
writeUIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var mul = 1;
  var i = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.expressions"></a>[module vogels.expressions](#apidoc.module.vogels.expressions)

#### <a name="apidoc.element.vogels.expressions.buildFilterExpression"></a>[function <span class="apidocSignatureSpan">vogels.expressions.</span>buildFilterExpression (key, operator, existingValueNames, val1, val2 )](#apidoc.element.vogels.expressions.buildFilterExpression)
- description and source-code
```javascript
buildFilterExpression = function (key, operator, existingValueNames, val1, val2 ) {
  // IN filter expression is unlike all the others where val1 is an array of values
  if (operator === 'IN') {
    return internals.buildInFilterExpression(key, existingValueNames, val1);
  }

  var v1 = internals.formatAttributeValue(val1);
  var v2 = internals.formatAttributeValue(val2);

  if (operator === 'attribute_exists' && v1 === false) {
    operator = 'attribute_not_exists';
    v1 = null;
  } else if (operator === 'attribute_exists' && v1 === true) {
    v1 = null;
  }

  var path = '#' + key;
  var v1ValueName = internals.uniqAttributeValueName(key, existingValueNames);
  var v2ValueName = internals.uniqAttributeValueName(key, [v1ValueName].concat(existingValueNames));

  var statement = '';

  if (internals.isFunctionOperator(operator)) {
    if (!_.isNull(v1) && !_.isUndefined(v1)) {
      statement = operator + '(' + path + ', ' + v1ValueName + ')';
    } else {
      statement = operator + '(' + path + ')';
    }
  } else if (operator === 'BETWEEN') {
    statement = path + ' BETWEEN ' + v1ValueName + ' AND ' + v2ValueName;
  } else {
    statement = [path, operator, v1ValueName].join(' ');
  }

  var attributeValues = {};

  if (!_.isNull(v1) && !_.isUndefined(v1)) {
    attributeValues[v1ValueName] = v1;
  }

  if (!_.isNull(v2) && !_.isUndefined(v2)) {
    attributeValues[v2ValueName] = v2;
  }

  var attributeNames = {};
  attributeNames[path] = key;

  return {
    attributeNames : attributeNames,
    statement : statement,
    attributeValues : attributeValues
  };
}
```
- example usage
```shell
...
var key = this.table.schema.hashKey;

if(internals.isUsingGlobalIndex(this)) {
  key = this.table.schema.globalIndexes[this.request.IndexName].hashKey;
}

var existingValueKeys = _.keys(this.request.ExpressionAttributeValues);
return expressions.buildFilterExpression(key, '=', existingValueKeys, this.hashKey);
};

internals.formatAttributeValue = function (val) {
if(_.isDate(val)) {
  return val.toISOString();
}
...
```

#### <a name="apidoc.element.vogels.expressions.parse"></a>[function <span class="apidocSignatureSpan">vogels.expressions.</span>parse (str)](#apidoc.element.vogels.expressions.parse)
- description and source-code
```javascript
parse = function (str) {
  return _.reduce(internals.actionWords, function (result, actionWord) {
    result[actionWord] = internals.match(actionWord, str);
    return result;
  }, {});
}
```
- example usage
```shell
...
  });
};

internals.updateExpressions = function (schema, data, options) {
  var exp = expressions.serializeUpdateExpression(schema, data);

  if(options.UpdateExpression) {
    var parsed = expressions.parse(options.UpdateExpression);

    exp.expressions = _.reduce(parsed, function (result, val, key) {
if(!_.isEmpty(val)) {
  result[key] = result[key].concat(val);
}

return result;
...
```

#### <a name="apidoc.element.vogels.expressions.serializeUpdateExpression"></a>[function <span class="apidocSignatureSpan">vogels.expressions.</span>serializeUpdateExpression (schema, item)](#apidoc.element.vogels.expressions.serializeUpdateExpression)
- description and source-code
```javascript
serializeUpdateExpression = function (schema, item) {
  var datatypes = schema._modelDatatypes;

  var data = utils.omitPrimaryKeys(schema, item);

  var memo = {
    expressions : {},
    attributeNames : {},
    values : {},
  };

  memo.expressions = _.reduce(internals.actionWords, function (result, key) {
    result[key] = [];

    return result;
  }, {});

  var result = _.reduce(data, function (result, value, key) {
    var valueKey = ':' + key;
    var nameKey = '#' + key;

    if(_.isNull(value) || (_.isString(value) && _.isEmpty(value)) ) {
      result.expressions.REMOVE.push(nameKey);
      result.attributeNames[nameKey] = key;
    } else if (_.isPlainObject(value) && value.$add) {
      result.expressions.ADD.push(nameKey + ' ' + valueKey);
      result.values[valueKey] = serializer.serializeAttribute(value.$add, datatypes[key]);
      result.attributeNames[nameKey] = key;
    } else if (_.isPlainObject(value) && value.$del) {
      result.expressions.DELETE.push(nameKey + ' ' + valueKey);
      result.values[valueKey] = serializer.serializeAttribute(value.$del, datatypes[key]);
      result.attributeNames[nameKey] = key;
    } else {
      result.expressions.SET.push(nameKey + ' = ' + valueKey);
      result.values[valueKey] = serializer.serializeAttribute(value, datatypes[key]);
      result.attributeNames[nameKey] = key;
    }

    return result;
  }, memo);

  return result;
}
```
- example usage
```shell
...

  return callback(null, item);
});
  });
};

internals.updateExpressions = function (schema, data, options) {
  var exp = expressions.serializeUpdateExpression(schema, data);

  if(options.UpdateExpression) {
var parsed = expressions.parse(options.UpdateExpression);

exp.expressions = _.reduce(parsed, function (result, val, key) {
  if(!_.isEmpty(val)) {
    result[key] = result[key].concat(val);
...
```

#### <a name="apidoc.element.vogels.expressions.stringify"></a>[function <span class="apidocSignatureSpan">vogels.expressions.</span>stringify (expressions)](#apidoc.element.vogels.expressions.stringify)
- description and source-code
```javascript
stringify = function (expressions) {
  return _.reduce(expressions, function (result, value, key) {
    if(!_.isEmpty(value)) {
      if(_.isArray(value)) {
        result.push(key + ' ' + value.join(', '));
      } else {
        result.push(key + ' ' + value);
      }
    }

    return result;
  }, []).join(' ');
}
```
- example usage
```shell
...
if(_.isPlainObject(options.ExpressionAttributeNames)) {
  exp.attributeNames = _.merge({}, exp.attributeNames, options.ExpressionAttributeNames);
}

return _.merge({}, {
  ExpressionAttributeValues : exp.values,
  ExpressionAttributeNames : exp.attributeNames,
  UpdateExpression : expressions.stringify(exp.expressions),
});
};

Table.prototype.update = function (item, options, callback) {
var self = this;

if (typeof options === 'function' && !callback) {
...
```



# <a name="apidoc.module.vogels.item"></a>[module vogels.item](#apidoc.module.vogels.item)

#### <a name="apidoc.element.vogels.item.item"></a>[function <span class="apidocSignatureSpan">vogels.</span>item (attrs, table)](#apidoc.element.vogels.item.item)
- description and source-code
```javascript
item = function (attrs, table) {
  events.EventEmitter.call(this);

  this.table = table;

  this.set(attrs || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.item.super_"></a>[function <span class="apidocSignatureSpan">vogels.item.</span>super_ ()](#apidoc.element.vogels.item.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.item.prototype"></a>[module vogels.item.prototype](#apidoc.module.vogels.item.prototype)

#### <a name="apidoc.element.vogels.item.prototype.destroy"></a>[function <span class="apidocSignatureSpan">vogels.item.prototype.</span>destroy (options, callback)](#apidoc.element.vogels.item.prototype.destroy)
- description and source-code
```javascript
destroy = function (options, callback) {
  var self = this;

  if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  options = options || {};
  callback = callback || internals.identity;

  self.table.destroy(this.attrs, options, callback);
}
```
- example usage
```shell
...
'''

### Deleting
You delete items in DynamoDB using the hashkey of model
If your model uses both a hash and range key, than both need to be provided

'''js
Account.destroy('foo@example.com', function (err) {
  console.log('account deleted');
});

// Destroy model using hash and range key
BlogPost.destroy('foo@example.com', 'Hello World!', function (err) {
  console.log('post deleted')
});
...
```

#### <a name="apidoc.element.vogels.item.prototype.get"></a>[function <span class="apidocSignatureSpan">vogels.item.prototype.</span>get (key)](#apidoc.element.vogels.item.prototype.get)
- description and source-code
```javascript
get = function (key) {
  if(key) {
    return this.attrs[key];
  } else {
    return this.attrs;
  }
}
```
- example usage
```shell
...
'''

### Saving Models to DynamoDB
With your models defined, we can start saving them to DynamoDB.

'''js
Account.create({email: 'foo@example.com', name: 'Foo Bar', age: 21}, function (err, acc) {
  console.log('created account in DynamoDB', acc.get('email'));
});
'''

You can also first instantiate a model and then save it.

'''js
var acc = new Account({email: 'test@example.com', name: 'Test Example'});
...
```

#### <a name="apidoc.element.vogels.item.prototype.save"></a>[function <span class="apidocSignatureSpan">vogels.item.prototype.</span>save (callback)](#apidoc.element.vogels.item.prototype.save)
- description and source-code
```javascript
save = function (callback) {
  var self = this;
  callback = callback || internals.identity;

  self.table.create(this.attrs, function (err, item) {
    if(err) {
      return callback(err);
    }

    self.set(item.attrs);

    return callback(null, item);
  });
}
```
- example usage
```shell
...
});
'''

You can also first instantiate a model and then save it.

'''js
var acc = new Account({email: 'test@example.com', name: 'Test Example'});
acc.save(function (err) {
  console.log('created account in DynamoDB', acc.get('email'));
});
'''

Saving models that require range and hashkeys are identical to ones with only
hashkeys.
...
```

#### <a name="apidoc.element.vogels.item.prototype.set"></a>[function <span class="apidocSignatureSpan">vogels.item.prototype.</span>set (params)](#apidoc.element.vogels.item.prototype.set)
- description and source-code
```javascript
set = function (params) {
  this.attrs = _.merge({}, this.attrs, params);

  return this;
}
```
- example usage
```shell
...
    age     : Joi.number(),
  }
});

Account.create({email: 'test@example.com', name : 'Test Account'}, function (err, acc) {
  console.log('created account at', acc.get('created')); // prints created Date

  acc.set({age: 22});

  acc.update(function (err) {
    console.log('updated account age');
  });

});
'''
...
```

#### <a name="apidoc.element.vogels.item.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">vogels.item.prototype.</span>toJSON ()](#apidoc.element.vogels.item.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return _.cloneDeep(this.attrs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.item.prototype.update"></a>[function <span class="apidocSignatureSpan">vogels.item.prototype.</span>update (options, callback)](#apidoc.element.vogels.item.prototype.update)
- description and source-code
```javascript
update = function (options, callback) {
  var self = this;

  if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  options = options || {};
  callback = callback || internals.identity;

  self.table.update(this.attrs, options, function (err, item) {
    if(err) {
      return callback(err);
    }

    if(item) {
      self.set(item.attrs);
    }

    return callback(null, item);
  });
}
```
- example usage
```shell
...
vogels.AWS.config.loadFromPath('credentials.json');
'''

When running on EC2 its recommended to leverage EC2 IAM roles. If you have configured your instance to use IAM roles, Vogels will
 automatically select these credentials for use in your application, and you do not need to manually provide credentials in any
other format.

'''js
var vogels = require('vogels');
vogels.AWS.config.update({region: "REGION"}); // region must be set
'''

You can also directly pass in your access key id, secret and region.
  * Its recommend you not hard-code credentials inside an application. Use this method only for small personal scripts or for testing
 purposes.

'''js
var vogels = require('vogels');
...
```



# <a name="apidoc.module.vogels.parallelScan"></a>[module vogels.parallelScan](#apidoc.module.vogels.parallelScan)

#### <a name="apidoc.element.vogels.parallelScan.parallelScan"></a>[function <span class="apidocSignatureSpan">vogels.</span>parallelScan (table, serializer, totalSegments)](#apidoc.element.vogels.parallelScan.parallelScan)
- description and source-code
```javascript
parallelScan = function (table, serializer, totalSegments) {
  Scan.call(this, table, serializer);

  this.totalSegments = totalSegments;
}
```
- example usage
```shell
...
The only difference is you must provide the total number of segments

**Caution** you can easily consume all your provisioned throughput with this api

'''js
var totalSegments = 8;

Account.parallelScan(totalSegments)
.where('age').gte(18)
.attributes('age')
.exec(callback);

// Load All accounts
Account
.parallelScan(totalSegments)
...
```

#### <a name="apidoc.element.vogels.parallelScan.super_"></a>[function <span class="apidocSignatureSpan">vogels.parallelScan.</span>super_ (table, serializer)](#apidoc.element.vogels.parallelScan.super_)
- description and source-code
```javascript
super_ = function (table, serializer) {
  this.table = table;
  this.serializer = serializer;
  this.options = {loadAll: false};

  this.request = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.parallelScan.prototype"></a>[module vogels.parallelScan.prototype](#apidoc.module.vogels.parallelScan.prototype)

#### <a name="apidoc.element.vogels.parallelScan.prototype.exec"></a>[function <span class="apidocSignatureSpan">vogels.parallelScan.prototype.</span>exec (callback)](#apidoc.element.vogels.parallelScan.prototype.exec)
- description and source-code
```javascript
exec = function (callback) {
  var self = this;

  var streamMode = false;
  var combinedStream = new Readable({objectMode: true});

  if(!callback) {
    streamMode = true;
    callback = function (err) {
      if(err) {
        combinedStream.emit('error', err);
      }
    };
  }

  var scanFuncs = [];
  _.times(self.totalSegments, function(segment) {
    var scn = new Scan(self.table, self.serializer);
    scn.request = _.cloneDeep(self.request);

    scn = scn.segments(segment, self.totalSegments).loadAll();

    var scanFunc = function (callback) {
      if(streamMode) {
        var stream = scn.exec();

        stream.on('error', callback);

        stream.on('readable', function () {
          var data = stream.read();
          if(data) {
            combinedStream.push(data);
          }
        });

        stream.on('end', callback);

      } else {
        return scn.exec(callback);
      }
    };

    scanFuncs.push(scanFunc);
  });

  var started = false;
  var startScans = function () {
    if(started) {
      return;
    }

    started = true;

    async.parallel(scanFuncs, function (err, responses) {
      if(err) {
        return callback(err);
      }

      combinedStream.push(null);
      return callback(null, utils.mergeResults(responses, self.table.tableName()));
    });
  };

  if(streamMode) {
    combinedStream._read = startScans;
  } else {
    startScans();
  }

  return combinedStream;
}
```
- example usage
```shell
...
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```



# <a name="apidoc.module.vogels.query"></a>[module vogels.query](#apidoc.module.vogels.query)

#### <a name="apidoc.element.vogels.query.query"></a>[function <span class="apidocSignatureSpan">vogels.</span>query (hashKey, table, serializer)](#apidoc.element.vogels.query.query)
- description and source-code
```javascript
query = function (hashKey, table, serializer) {
  this.hashKey = hashKey;
  this.table = table;
  this.serializer = serializer;

  this.options = {loadAll: false};
  this.request = {};
}
```
- example usage
```shell
...
### Query
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```



# <a name="apidoc.module.vogels.query.prototype"></a>[module vogels.query.prototype](#apidoc.module.vogels.query.prototype)

#### <a name="apidoc.element.vogels.query.prototype.addFilterCondition"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>addFilterCondition (condition)](#apidoc.element.vogels.query.prototype.addFilterCondition)
- description and source-code
```javascript
addFilterCondition = function (condition) {
  internals.addExpressionAttributes(this.request, condition);

  if (_.isString(this.request.FilterExpression )) {
    this.request.FilterExpression = this.request.FilterExpression + ' AND (' + condition.statement + ')';
  } else {
    this.request.FilterExpression = '(' + condition.statement + ')';
  }

  return this;
}
```
- example usage
```shell
...

var f = function (operator) {
  return function (/*values*/) {
    var copy = [].slice.call(arguments);
    var existingValueKeys = _.keys(query.request.ExpressionAttributeValues);
    var args = [keyName, operator, existingValueKeys].concat(copy);
    var cond = expressions.buildFilterExpression.apply(null, args);
    return query.addFilterCondition(cond);
  };
};

return {
  equals      : f('='),
  eq          : f('='),
  ne          : f('<>'),
...
```

#### <a name="apidoc.element.vogels.query.prototype.addKeyCondition"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>addKeyCondition (condition)](#apidoc.element.vogels.query.prototype.addKeyCondition)
- description and source-code
```javascript
addKeyCondition = function (condition) {
  internals.addExpressionAttributes(this.request, condition);

  if (_.isString(this.request.KeyConditionExpression )) {
    this.request.KeyConditionExpression = this.request.KeyConditionExpression + ' AND (' + condition.statement + ')';
  } else {
    this.request.KeyConditionExpression = '(' + condition.statement + ')';
  }

  return this;
}
```
- example usage
```shell
...

var f = function (operator) {
  return function (/*values*/) {
    var copy = [].slice.call(arguments);
    var existingValueKeys = _.keys(query.request.ExpressionAttributeValues);
    var args = [keyName, operator, existingValueKeys].concat(copy);
    var cond = expressions.buildFilterExpression.apply(null, args);
    return query.addKeyCondition(cond);
  };
};

return {
  equals      : f('='),
  eq          : f('='),
  lte         : f('<='),
...
```

#### <a name="apidoc.element.vogels.query.prototype.ascending"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>ascending ()](#apidoc.element.vogels.query.prototype.ascending)
- description and source-code
```javascript
ascending = function () {
  this.request.ScanIndexForward = true;

  return this;
}
```
- example usage
```shell
...
.attributes(['title', 'content'])
.limit(10)
.exec(callback);

// sorting by title ascending
BlogPost
.query('werner@example.com')
.ascending()
.exec(callback)

// sorting by title descending
BlogPost
.query('werner@example.com')
.descending()
.exec(callback)
...
```

#### <a name="apidoc.element.vogels.query.prototype.attributes"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>attributes (attrs)](#apidoc.element.vogels.query.prototype.attributes)
- description and source-code
```javascript
attributes = function (attrs) {
  if(!_.isArray(attrs)) {
    attrs = [attrs];
  }

  var expressionAttributeNames = _.reduce(attrs, function (result, attr) {
    var path = '#' + attr;
    result[path] = attr;

    return result;
  }, {});

  this.request.ProjectionExpression = _.keys(expressionAttributeNames).join(',');
  this.request.ExpressionAttributeNames = _.merge({}, expressionAttributeNames, this.request.ExpressionAttributeNames);

  return this;
}
```
- example usage
```shell
...
.exec(callback);

// only return title and content attributes of 10 blog posts
// that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.attributes(['title', 'content'])
.limit(10)
.exec(callback);

// sorting by title ascending
BlogPost
.query('werner@example.com')
.ascending()
...
```

#### <a name="apidoc.element.vogels.query.prototype.buildKey"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>buildKey ()](#apidoc.element.vogels.query.prototype.buildKey)
- description and source-code
```javascript
buildKey = function () {
  var key = this.table.schema.hashKey;

  if(internals.isUsingGlobalIndex(this)) {
    key = this.table.schema.globalIndexes[this.request.IndexName].hashKey;
  }

  var existingValueKeys = _.keys(this.request.ExpressionAttributeValues);
  return expressions.buildFilterExpression(key, '=', existingValueKeys, this.hashKey);
}
```
- example usage
```shell
...
request[tableName] = _.merge({}, {Keys : keys}, options);

return { RequestItems : request };
};

internals.serializeKeys = function (keys, table, serializer) {
return keys.map(function (key) {
  return serializer.buildKey(key, null, table.schema);
});
};

internals.mergeResponses = function (tableName, responses) {
var base = {
  Responses : {},
  ConsumedCapacity : []
...
```

#### <a name="apidoc.element.vogels.query.prototype.buildRequest"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>buildRequest ()](#apidoc.element.vogels.query.prototype.buildRequest)
- description and source-code
```javascript
buildRequest = function () {
  return _.merge({}, this.request, {TableName: this.table.tableName()});
}
```
- example usage
```shell
...
  var retry = false;

  var doFunc = function (callback) {
if(lastEvaluatedKey) {
  self.startKey(lastEvaluatedKey);
}

runRequestFunc(self.buildRequest(), function (err, resp) {
  if(err && err.retryable) {
    retry = true;
    return setImmediate(callback);
  } else if(err) {
    retry = false;
    return setImmediate(callback, err);
  }
...
```

#### <a name="apidoc.element.vogels.query.prototype.consistentRead"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>consistentRead (read)](#apidoc.element.vogels.query.prototype.consistentRead)
- description and source-code
```javascript
consistentRead = function (read) {
  if(!_.isBoolean(read)) {
    read = true;
  }

  this.request.ConsistentRead = read;

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.query.prototype.descending"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>descending ()](#apidoc.element.vogels.query.prototype.descending)
- description and source-code
```javascript
descending = function () {
  this.request.ScanIndexForward = false;

  return this;
}
```
- example usage
```shell
...
.query('werner@example.com')
.ascending()
.exec(callback)

// sorting by title descending
BlogPost
.query('werner@example.com')
.descending()
.exec(callback)

// All query options are chainable
BlogPost
.query('werner@example.com')
.where('title').gt('Expanding')
.attributes(['title', 'content'])
...
```

#### <a name="apidoc.element.vogels.query.prototype.exec"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>exec (callback)](#apidoc.element.vogels.query.prototype.exec)
- description and source-code
```javascript
exec = function (callback) {
  var self = this;

  this.addKeyCondition(this.buildKey());

  var runQuery = function (params, callback) {
    self.table.runQuery(params, callback);
  };

  return utils.paginatedRequest(self, runQuery, callback);
}
```
- example usage
```shell
...
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.query.prototype.expressionAttributeNames"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>expressionAttributeNames (data)](#apidoc.element.vogels.query.prototype.expressionAttributeNames)
- description and source-code
```javascript
expressionAttributeNames = function (data) {
  this.request.ExpressionAttributeNames = data;

  return this;
}
```
- example usage
```shell
...
Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters

#### Global Indexes
...
```

#### <a name="apidoc.element.vogels.query.prototype.expressionAttributeValues"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>expressionAttributeValues (data)](#apidoc.element.vogels.query.prototype.expressionAttributeValues)
- description and source-code
```javascript
expressionAttributeValues = function (data) {
  this.request.ExpressionAttributeValues = data;

  return this;
}
```
- example usage
```shell
...

Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters
...
```

#### <a name="apidoc.element.vogels.query.prototype.filter"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>filter (keyName)](#apidoc.element.vogels.query.prototype.filter)
- description and source-code
```javascript
filter = function (keyName) {
  return internals.queryFilter(keyName, this.table.schema, this);
}
```
- example usage
```shell
...

Query Filters allow you to further filter results on non-key attributes.

'''js
BlogPost
  .query('werner@example.com')
  .where('title').equals('Expanding')
  .filter('tags').contains('cloud')
  .exec();
'''

Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
...
```

#### <a name="apidoc.element.vogels.query.prototype.filterExpression"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>filterExpression (expression)](#apidoc.element.vogels.query.prototype.filterExpression)
- description and source-code
```javascript
filterExpression = function (expression) {
  this.request.FilterExpression = expression;

  return this;
}
```
- example usage
```shell
...
'''

Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters
...
```

#### <a name="apidoc.element.vogels.query.prototype.limit"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>limit (num)](#apidoc.element.vogels.query.prototype.limit)
- description and source-code
```javascript
limit = function (num) {
  if(num <= 0 ) {
    throw new Error('Limit must be greater than 0');
  }

  this.request.Limit = num;

  return this;
}
```
- example usage
```shell
...
.query('werner@example.com')
.loadAll()
.exec(callback);

// only load the first 5 posts by werner
BlogPost
.query('werner@example.com')
.limit(5)
.exec(callback);

// query for posts by werner where the tile begins with 'Expanding'
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.query.prototype.loadAll"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>loadAll ()](#apidoc.element.vogels.query.prototype.loadAll)
- description and source-code
```javascript
loadAll = function () {
  this.options.loadAll = true;

  return this;
}
```
- example usage
```shell
...
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);

// only load the first 5 posts by werner
BlogPost
.query('werner@example.com')
.limit(5)
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.query.prototype.projectionExpression"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>projectionExpression (data)](#apidoc.element.vogels.query.prototype.projectionExpression)
- description and source-code
```javascript
projectionExpression = function (data) {
  this.request.ProjectionExpression = data;

  return this;
}
```
- example usage
```shell
...

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters

#### Global Indexes
First, define a model with a global secondary index.
...
```

#### <a name="apidoc.element.vogels.query.prototype.returnConsumedCapacity"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>returnConsumedCapacity (value)](#apidoc.element.vogels.query.prototype.returnConsumedCapacity)
- description and source-code
```javascript
returnConsumedCapacity = function (value) {
  if(_.isUndefined(value)) {
    value = 'TOTAL';
  }

  this.request.ReturnConsumedCapacity = value;

  return this;
}
```
- example usage
```shell
...
// Load accounts which match a filter
// only return email and created attributes
// and return back the consumed capacity the request took
Account
.scan()
.where('email').gte('f@example.com')
.attributes(['email','created'])
.returnConsumedCapacity()
.exec();

// Returns number of matching accounts, rather than the matching accounts themselves
Account
.scan()
.where('age').gte(21)
.select('COUNT')
...
```

#### <a name="apidoc.element.vogels.query.prototype.select"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>select (value)](#apidoc.element.vogels.query.prototype.select)
- description and source-code
```javascript
select = function (value) {
  this.request.Select = value;

  return this;
}
```
- example usage
```shell
...
.where('title').beginsWith('Expanding')
.exec(callback);

// return only the count of documents that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.select('COUNT')
.exec(callback);

// only return title and content attributes of 10 blog posts
// that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
...
```

#### <a name="apidoc.element.vogels.query.prototype.startKey"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>startKey (hashKey, rangeKey)](#apidoc.element.vogels.query.prototype.startKey)
- description and source-code
```javascript
startKey = function (hashKey, rangeKey) {
  this.request.ExclusiveStartKey = this.serializer.buildKey(hashKey, rangeKey, this.table.schema);

  return this;
}
```
- example usage
```shell
...
  .select('COUNT')
  .exec();

// Start scan using start key
Account
  .scan()
  .where('age').notNull()
  .startKey('foo@example.com')
  .exec()
'''

Vogels supports all the possible Scan Filters that DynamoDB currently supports.

'''js
// equals
...
```

#### <a name="apidoc.element.vogels.query.prototype.usingIndex"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>usingIndex (name)](#apidoc.element.vogels.query.prototype.usingIndex)
- description and source-code
```javascript
usingIndex = function (name) {
  this.request.IndexName = name;

  return this;
}
```
- example usage
```shell
...
'''

Now we can query against the global index

'''js
GameScore
  .query('Galaxy Invaders')
  .usingIndex('GameTitleIndex')
  .descending()
  .exec(callback);
'''

When can also configure the attributes projected into the index.
By default all attributes will be projected when no Projection pramater is
present
...
```

#### <a name="apidoc.element.vogels.query.prototype.where"></a>[function <span class="apidocSignatureSpan">vogels.query.prototype.</span>where (keyName)](#apidoc.element.vogels.query.prototype.where)
- description and source-code
```javascript
where = function (keyName) {
  return internals.keyCondition(keyName, this.table.schema, this);
}
```
- example usage
```shell
...
.query('werner@example.com')
.limit(5)
.exec(callback);

// query for posts by werner where the tile begins with 'Expanding'
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.exec(callback);

// return only the count of documents that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.select('COUNT')
...
```



# <a name="apidoc.module.vogels.scan"></a>[module vogels.scan](#apidoc.module.vogels.scan)

#### <a name="apidoc.element.vogels.scan.scan"></a>[function <span class="apidocSignatureSpan">vogels.</span>scan (table, serializer)](#apidoc.element.vogels.scan.scan)
- description and source-code
```javascript
scan = function (table, serializer) {
  this.table = table;
  this.serializer = serializer;
  this.options = {loadAll: false};

  this.request = {};
}
```
- example usage
```shell
...

### Scan
Vogels provides a flexible and chainable api for scanning over all your items
This api is very similar to the query api.

'''js
// scan all accounts, returning the first page or results
Account.scan().exec(callback);

// scan all accounts, this time loading all results
// note this will potentially make several calls to DynamoDB
// in order to load all results
Account
.scan()
.loadAll()
...
```



# <a name="apidoc.module.vogels.scan.prototype"></a>[module vogels.scan.prototype](#apidoc.module.vogels.scan.prototype)

#### <a name="apidoc.element.vogels.scan.prototype.addFilterCondition"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>addFilterCondition (condition)](#apidoc.element.vogels.scan.prototype.addFilterCondition)
- description and source-code
```javascript
addFilterCondition = function (condition) {
  var expressionAttributeNames  = _.merge({}, condition.attributeNames, this.request.ExpressionAttributeNames);
  var expressionAttributeValues = _.merge({}, condition.attributeValues, this.request.ExpressionAttributeValues);

  if (!_.isEmpty(expressionAttributeNames)) {
    this.request.ExpressionAttributeNames = expressionAttributeNames;
  }

  if (!_.isEmpty(expressionAttributeValues)) {
    this.request.ExpressionAttributeValues = expressionAttributeValues;
  }

  if (_.isString(this.request.FilterExpression )) {
    this.request.FilterExpression = this.request.FilterExpression + ' AND (' + condition.statement + ')';
  } else {
    this.request.FilterExpression = '(' + condition.statement + ')';
  }

  return this;
}
```
- example usage
```shell
...

var f = function (operator) {
  return function (/*values*/) {
    var copy = [].slice.call(arguments);
    var existingValueKeys = _.keys(query.request.ExpressionAttributeValues);
    var args = [keyName, operator, existingValueKeys].concat(copy);
    var cond = expressions.buildFilterExpression.apply(null, args);
    return query.addFilterCondition(cond);
  };
};

return {
  equals      : f('='),
  eq          : f('='),
  ne          : f('<>'),
...
```

#### <a name="apidoc.element.vogels.scan.prototype.attributes"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>attributes (attrs)](#apidoc.element.vogels.scan.prototype.attributes)
- description and source-code
```javascript
attributes = function (attrs) {
  if(!_.isArray(attrs)) {
    attrs = [attrs];
  }

  var expressionAttributeNames = _.reduce(attrs, function (result, attr) {
    var path = '#' + attr;
    result[path] = attr;

    return result;
  }, {});

  this.request.ProjectionExpression = _.keys(expressionAttributeNames).join(',');
  this.request.ExpressionAttributeNames = _.merge({}, expressionAttributeNames, this.request.ExpressionAttributeNames);

  return this;
}
```
- example usage
```shell
...
.exec(callback);

// only return title and content attributes of 10 blog posts
// that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.attributes(['title', 'content'])
.limit(10)
.exec(callback);

// sorting by title ascending
BlogPost
.query('werner@example.com')
.ascending()
...
```

#### <a name="apidoc.element.vogels.scan.prototype.buildRequest"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>buildRequest ()](#apidoc.element.vogels.scan.prototype.buildRequest)
- description and source-code
```javascript
buildRequest = function () {
  return _.merge({}, this.request, {TableName: this.table.tableName()});
}
```
- example usage
```shell
...
  var retry = false;

  var doFunc = function (callback) {
if(lastEvaluatedKey) {
  self.startKey(lastEvaluatedKey);
}

runRequestFunc(self.buildRequest(), function (err, resp) {
  if(err && err.retryable) {
    retry = true;
    return setImmediate(callback);
  } else if(err) {
    retry = false;
    return setImmediate(callback, err);
  }
...
```

#### <a name="apidoc.element.vogels.scan.prototype.exec"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>exec (callback)](#apidoc.element.vogels.scan.prototype.exec)
- description and source-code
```javascript
exec = function (callback) {
  var self = this;

  var runScan = function (params, callback) {
    self.table.runScan(params, callback);
  };

  return utils.paginatedRequest(self, runScan, callback);
}
```
- example usage
```shell
...
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.scan.prototype.expressionAttributeNames"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>expressionAttributeNames (data)](#apidoc.element.vogels.scan.prototype.expressionAttributeNames)
- description and source-code
```javascript
expressionAttributeNames = function (data) {
  this.request.ExpressionAttributeNames = data;

  return this;
}
```
- example usage
```shell
...
Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters

#### Global Indexes
...
```

#### <a name="apidoc.element.vogels.scan.prototype.expressionAttributeValues"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>expressionAttributeValues (data)](#apidoc.element.vogels.scan.prototype.expressionAttributeValues)
- description and source-code
```javascript
expressionAttributeValues = function (data) {
  this.request.ExpressionAttributeValues = data;

  return this;
}
```
- example usage
```shell
...

Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters
...
```

#### <a name="apidoc.element.vogels.scan.prototype.filterExpression"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>filterExpression (expression)](#apidoc.element.vogels.scan.prototype.filterExpression)
- description and source-code
```javascript
filterExpression = function (expression) {
  this.request.FilterExpression = expression;

  return this;
}
```
- example usage
```shell
...
'''

Expression Filters also allow you to further filter results on non-key attributes.

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters
...
```

#### <a name="apidoc.element.vogels.scan.prototype.limit"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>limit (num)](#apidoc.element.vogels.scan.prototype.limit)
- description and source-code
```javascript
limit = function (num) {
  if(num <= 0 ) {
    throw new Error('Limit must be greater than 0');
  }

  this.request.Limit = num;

  return this;
}
```
- example usage
```shell
...
.query('werner@example.com')
.loadAll()
.exec(callback);

// only load the first 5 posts by werner
BlogPost
.query('werner@example.com')
.limit(5)
.exec(callback);

// query for posts by werner where the tile begins with 'Expanding'
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.scan.prototype.loadAll"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>loadAll ()](#apidoc.element.vogels.scan.prototype.loadAll)
- description and source-code
```javascript
loadAll = function () {
  this.options.loadAll = true;

  return this;
}
```
- example usage
```shell
...
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);

// only load the first 5 posts by werner
BlogPost
.query('werner@example.com')
.limit(5)
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.scan.prototype.projectionExpression"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>projectionExpression (data)](#apidoc.element.vogels.scan.prototype.projectionExpression)
- description and source-code
```javascript
projectionExpression = function (data) {
  this.request.ProjectionExpression = data;

  return this;
}
```
- example usage
```shell
...

'''javascript
BlogPost
  .query('werner@example.com')
  .filterExpression('#title < :t')
  .expressionAttributeValues({ ':t' : 'Expanding' })
  .expressionAttributeNames({ '#title' : 'title'})
  .projectionExpression('#title, tag')
  .exec();
'''

See the queryFilter.js [example][0] for more examples of using query filters

#### Global Indexes
First, define a model with a global secondary index.
...
```

#### <a name="apidoc.element.vogels.scan.prototype.returnConsumedCapacity"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>returnConsumedCapacity (value)](#apidoc.element.vogels.scan.prototype.returnConsumedCapacity)
- description and source-code
```javascript
returnConsumedCapacity = function (value) {
  if(_.isUndefined(value)) {
    value = 'TOTAL';
  }

  this.request.ReturnConsumedCapacity = value;

  return this;
}
```
- example usage
```shell
...
// Load accounts which match a filter
// only return email and created attributes
// and return back the consumed capacity the request took
Account
.scan()
.where('email').gte('f@example.com')
.attributes(['email','created'])
.returnConsumedCapacity()
.exec();

// Returns number of matching accounts, rather than the matching accounts themselves
Account
.scan()
.where('age').gte(21)
.select('COUNT')
...
```

#### <a name="apidoc.element.vogels.scan.prototype.segments"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>segments (segment, totalSegments)](#apidoc.element.vogels.scan.prototype.segments)
- description and source-code
```javascript
segments = function (segment, totalSegments) {
  this.request.Segment = segment;
  this.request.TotalSegments = totalSegments;

  return this;
}
```
- example usage
```shell
...
  }

  var scanFuncs = [];
  _.times(self.totalSegments, function(segment) {
    var scn = new Scan(self.table, self.serializer);
    scn.request = _.cloneDeep(self.request);

    scn = scn.segments(segment, self.totalSegments).loadAll();

    var scanFunc = function (callback) {
      if(streamMode) {
var stream = scn.exec();

stream.on('error', callback);
...
```

#### <a name="apidoc.element.vogels.scan.prototype.select"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>select (value)](#apidoc.element.vogels.scan.prototype.select)
- description and source-code
```javascript
select = function (value) {
  this.request.Select = value;

  return this;
}
```
- example usage
```shell
...
.where('title').beginsWith('Expanding')
.exec(callback);

// return only the count of documents that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.select('COUNT')
.exec(callback);

// only return title and content attributes of 10 blog posts
// that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
...
```

#### <a name="apidoc.element.vogels.scan.prototype.startKey"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>startKey (hashKey, rangeKey)](#apidoc.element.vogels.scan.prototype.startKey)
- description and source-code
```javascript
startKey = function (hashKey, rangeKey) {
  this.request.ExclusiveStartKey = this.serializer.buildKey(hashKey, rangeKey, this.table.schema);

  return this;
}
```
- example usage
```shell
...
  .select('COUNT')
  .exec();

// Start scan using start key
Account
  .scan()
  .where('age').notNull()
  .startKey('foo@example.com')
  .exec()
'''

Vogels supports all the possible Scan Filters that DynamoDB currently supports.

'''js
// equals
...
```

#### <a name="apidoc.element.vogels.scan.prototype.where"></a>[function <span class="apidocSignatureSpan">vogels.scan.prototype.</span>where (keyName)](#apidoc.element.vogels.scan.prototype.where)
- description and source-code
```javascript
where = function (keyName) {
  return internals.keyCondition(keyName, this.table.schema, this);
}
```
- example usage
```shell
...
.query('werner@example.com')
.limit(5)
.exec(callback);

// query for posts by werner where the tile begins with 'Expanding'
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.exec(callback);

// return only the count of documents that begin with the title Expanding
BlogPost
.query('werner@example.com')
.where('title').beginsWith('Expanding')
.select('COUNT')
...
```



# <a name="apidoc.module.vogels.schema"></a>[module vogels.schema](#apidoc.module.vogels.schema)

#### <a name="apidoc.element.vogels.schema.schema"></a>[function <span class="apidocSignatureSpan">vogels.</span>schema (config)](#apidoc.element.vogels.schema.schema)
- description and source-code
```javascript
schema = function (config) {
  this.secondaryIndexes = {};
  this.globalIndexes = {};

  var context = {hashKey : config.hashKey};

  var self = this;
  Joi.validate(config, internals.configSchema, { context: context }, function (err, data) {
    if(err) {
      var msg = 'Invalid table schema, check your config ';
      throw new Error(msg + err.annotate());
    }

    self.hashKey    = data.hashKey;
    self.rangeKey   = data.rangeKey;
    self.tableName  = data.tableName;
    self.timestamps = data.timestamps;
    self.createdAt  = data.createdAt;
    self.updatedAt  = data.updatedAt;

    if(data.indexes) {
      self.globalIndexes    = _.chain(data.indexes).filter({ type: 'global' }).indexBy('name').value();
      self.secondaryIndexes = _.chain(data.indexes).filter({ type: 'local' }).indexBy('name').value();
    }

    if(data.schema) {
      self._modelSchema    = _.isPlainObject(data.schema) ? Joi.object().keys(data.schema) : data.schema;
    } else {
      self._modelSchema = Joi.object();
    }

    if(self.timestamps) {
      var valids = {};
      var createdAtParamName = 'createdAt';
      var updatedAtParamName = 'updatedAt';

      if(self.createdAt) {
        if(_.isString(self.createdAt)) {
          createdAtParamName = self.createdAt;
        }
      }

      if(self.updatedAt) {
        if(_.isString(self.updatedAt)) {
          updatedAtParamName = self.updatedAt;
        }
      }

      if(self.createdAt !== false) {
        valids[createdAtParamName] = Joi.date();
      }

      if(self.updatedAt !== false) {
        valids[updatedAtParamName] = Joi.date();
      }

      var extended = self._modelSchema.keys(valids);

      self._modelSchema = extended;
    }

    self._modelDatatypes = internals.parseDynamoTypes(self._modelSchema.describe());
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.schema.prototype"></a>[module vogels.schema.prototype](#apidoc.module.vogels.schema.prototype)

#### <a name="apidoc.element.vogels.schema.prototype.applyDefaults"></a>[function <span class="apidocSignatureSpan">vogels.schema.prototype.</span>applyDefaults (data)](#apidoc.element.vogels.schema.prototype.applyDefaults)
- description and source-code
```javascript
applyDefaults = function (data) {
  var result = this.validate(data, {abortEarly : false});

  return internals.invokeDefaultFunctions(result.value);
}
```
- example usage
```shell
...
  }
};

internals.createItem = function (table, item, options, callback) {
  var self = table;

  var start = function (callback) {
var data = self.schema.applyDefaults(item);

var paramName = _.isString(self.schema.createdAt) ? self.schema.createdAt : 'createdAt';

if(self.schema.timestamps && self.schema.createdAt !== false && !_.has(data, paramName)) {
  data[paramName] = new Date().toISOString();
}
...
```

#### <a name="apidoc.element.vogels.schema.prototype.validate"></a>[function <span class="apidocSignatureSpan">vogels.schema.prototype.</span>validate (params, options)](#apidoc.element.vogels.schema.prototype.validate)
- description and source-code
```javascript
validate = function (params, options) {
  options = options || {};

  return Joi.validate(params, this._modelSchema, options);
}
```
- example usage
```shell
...
var Schema = module.exports = function (config) {
  this.secondaryIndexes = {};
  this.globalIndexes = {};

  var context = {hashKey : config.hashKey};

  var self = this;
  Joi.validate(config, internals.configSchema, { context: context }, function (err, data) {
if(err) {
  var msg = 'Invalid table schema, check your config ';
  throw new Error(msg + err.annotate());
}

self.hashKey    = data.hashKey;
self.rangeKey   = data.rangeKey;
...
```



# <a name="apidoc.module.vogels.serializer"></a>[module vogels.serializer](#apidoc.module.vogels.serializer)

#### <a name="apidoc.element.vogels.serializer.buildKey"></a>[function <span class="apidocSignatureSpan">vogels.serializer.</span>buildKey (hashKey, rangeKey, schema)](#apidoc.element.vogels.serializer.buildKey)
- description and source-code
```javascript
buildKey = function (hashKey, rangeKey, schema) {
  var obj = {};

  if(_.isPlainObject(hashKey)) {
    obj[schema.hashKey] = hashKey[schema.hashKey];

    if(schema.rangeKey && !_.isNull(hashKey[schema.rangeKey]) && !_.isUndefined(hashKey[schema.rangeKey])) {
      obj[schema.rangeKey] = hashKey[schema.rangeKey];
    }
    _.each(schema.globalIndexes, function (keys) {
      if(_.has(hashKey, keys.hashKey)){
        obj[keys.hashKey] = hashKey[keys.hashKey];
      }

      if(_.has(hashKey, keys.rangeKey)){
        obj[keys.rangeKey] = hashKey[keys.rangeKey];
      }
    });

    _.each(schema.secondaryIndexes, function (keys) {
      if(_.has(hashKey, keys.rangeKey)){
        obj[keys.rangeKey] = hashKey[keys.rangeKey];
      }
    });

  } else {
    obj[schema.hashKey] = hashKey;

    if(schema.rangeKey && !_.isNull(rangeKey) && !_.isUndefined(rangeKey)) {
      obj[schema.rangeKey] = rangeKey;
    }
  }

  return serializer.serializeItem(schema, obj);
}
```
- example usage
```shell
...
request[tableName] = _.merge({}, {Keys : keys}, options);

return { RequestItems : request };
};

internals.serializeKeys = function (keys, table, serializer) {
return keys.map(function (key) {
  return serializer.buildKey(key, null, table.schema);
});
};

internals.mergeResponses = function (tableName, responses) {
var base = {
  Responses : {},
  ConsumedCapacity : []
...
```

#### <a name="apidoc.element.vogels.serializer.deserializeItem"></a>[function <span class="apidocSignatureSpan">vogels.serializer.</span>deserializeItem (item)](#apidoc.element.vogels.serializer.deserializeItem)
- description and source-code
```javascript
deserializeItem = function (item) {

  if(_.isNull(item)) {
    return null;
  }

  var formatter = function (data) {
    var map = _.mapValues;

    if(_.isArray(data)) {
      map = _.map;
    }

    return map(data, function(value) {
      var result;

      if(_.isPlainObject(value)) {
        result = formatter(value);
      } else if(_.isArray(value)) {
        result = formatter(value);
      } else {
        result = internals.deserializeAttribute(value);
      }

      return result;
    });
  };

  return formatter(item);
}
```
- example usage
```shell
...
    if(err) {
      return callback(err);
    }

    var dynamoItems = data.Responses[table.tableName()];

    var items = _.map(dynamoItems, function(i) {
      return table.initItem(serializer.deserializeItem(i));
    });

    return callback(null, items);
  });
};

internals.getItems = function (table, serializer) {
...
```

#### <a name="apidoc.element.vogels.serializer.serializeAttribute"></a>[function <span class="apidocSignatureSpan">vogels.serializer.</span>serializeAttribute (value, type, options)](#apidoc.element.vogels.serializer.serializeAttribute)
- description and source-code
```javascript
serializeAttribute = function (value, type, options) {
  if(!type) { // if type is unknown, possibly because its an dynamic key return given value
    return value;
  }

  if(_.isNull(value)) {
    return null;
  }

  options = options || {};

  switch(type){
  case 'DATE':
    return serialize.date(value);
  case 'BOOL':
    return serialize.boolean(value);
  case 'B':
    return serialize.binary(value);
  case 'NS':
    return serialize.numberSet(value);
  case 'SS':
    return serialize.stringSet(value);
  case 'BS':
    return serialize.binarySet(value);
  default:
    return value;
  }
}
```
- example usage
```shell
...
var nameKey = '#' + key;

if(_.isNull(value) || (_.isString(value) && _.isEmpty(value)) ) {
  result.expressions.REMOVE.push(nameKey);
  result.attributeNames[nameKey] = key;
} else if (_.isPlainObject(value) && value.$add) {
  result.expressions.ADD.push(nameKey + ' ' + valueKey);
  result.values[valueKey] = serializer.serializeAttribute(value.$add, datatypes[key]);
  result.attributeNames[nameKey] = key;
} else if (_.isPlainObject(value) && value.$del) {
  result.expressions.DELETE.push(nameKey + ' ' + valueKey);
  result.values[valueKey] = serializer.serializeAttribute(value.$del, datatypes[key]);
  result.attributeNames[nameKey] = key;
} else {
  result.expressions.SET.push(nameKey + ' = ' + valueKey);
...
```

#### <a name="apidoc.element.vogels.serializer.serializeItem"></a>[function <span class="apidocSignatureSpan">vogels.serializer.</span>serializeItem (schema, item, options)](#apidoc.element.vogels.serializer.serializeItem)
- description and source-code
```javascript
serializeItem = function (schema, item, options) {
  options = options || {};

  var serialize = function (item, datatypes) {
    datatypes = datatypes || {};

    if(!item) {
      return null;
    }

    return _.reduce(item, function (result, val, key) {
      if(options.expected && _.isObject(val) && _.isBoolean(val.Exists)) {
        result[key] = val;
        return result;
      }

      if(_.isPlainObject(val)) {
        result[key] = serialize(val, datatypes[key]);
        return result;
      }

      var attr = internals.serializeAttribute(val, datatypes[key], options);

      if(!_.isNull(attr) || options.returnNulls) {
        if(options.expected) {
          result[key] = {'Value' : attr};
        } else {
          result[key] = attr;
        }
      }

      return result;
    }, {});
  };

  return serialize(item, schema._modelDatatypes);
}
```
- example usage
```shell
...
  obj[schema.hashKey] = hashKey;

  if(schema.rangeKey && !_.isNull(rangeKey) && !_.isUndefined(rangeKey)) {
    obj[schema.rangeKey] = rangeKey;
  }
}

return serializer.serializeItem(schema, obj);
};

serializer.serializeItem = function (schema, item, options) {
options = options || {};

var serialize = function (item, datatypes) {
  datatypes = datatypes || {};
...
```

#### <a name="apidoc.element.vogels.serializer.serializeItemForUpdate"></a>[function <span class="apidocSignatureSpan">vogels.serializer.</span>serializeItemForUpdate (schema, action, item)](#apidoc.element.vogels.serializer.serializeItemForUpdate)
- description and source-code
```javascript
serializeItemForUpdate = function (schema, action, item) {
  var datatypes = schema._modelDatatypes;

  var data = utils.omitPrimaryKeys(schema, item);
  return _.reduce(data, function (result, value, key) {
    if(_.isNull(value)) {
      result[key] = {Action : 'DELETE'};
    } else if (_.isPlainObject(value) && value.$add) {
      result[key] = {Action : 'ADD', Value: internals.serializeAttribute(value.$add, datatypes[key])};
    } else if (_.isPlainObject(value) && value.$del) {
      result[key] = {Action : 'DELETE', Value: internals.serializeAttribute(value.$del, datatypes[key])};
    } else {
      result[key] =  {Action : action, Value: internals.serializeAttribute(value, datatypes[key])};
    }

    return result;
  }, {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.table"></a>[module vogels.table](#apidoc.module.vogels.table)

#### <a name="apidoc.element.vogels.table.table"></a>[function <span class="apidocSignatureSpan">vogels.</span>table (name, schema, serializer, docClient, logger)](#apidoc.element.vogels.table.table)
- description and source-code
```javascript
table = function (name, schema, serializer, docClient, logger) {
  this.config = {name : name};
  this.schema = schema;
  this.serializer = serializer;
  this.docClient = docClient;
  this.log = logger;

  this._before = new EventEmitter();
  this.before = this._before.on.bind(this._before);

  this._after= new EventEmitter();
  this.after = this._after.on.bind(this._after);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vogels.table.prototype"></a>[module vogels.table.prototype](#apidoc.module.vogels.table.prototype)

#### <a name="apidoc.element.vogels.table.prototype.create"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>create (item, options, callback)](#apidoc.element.vogels.table.prototype.create)
- description and source-code
```javascript
create = function (item, options, callback) {
  var self = this;

  if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  callback = callback || _.noop;
  options = options || {};

  if (_.isArray(item)) {
    async.map(item, function (data, callback) {
      return internals.createItem(self, data, options, callback);
    }, callback);
  } else {
    return internals.createItem(self, item, options, callback);
  }
}
```
- example usage
```shell
...
vogels.dynamoDriver(dynamodb);
'''

### Saving Models to DynamoDB
With your models defined, we can start saving them to DynamoDB.

'''js
Account.create({email: 'foo@example.com', name: 'Foo Bar', age: 21}, function (err, acc) {
  console.log('created account in DynamoDB', acc.get('email'));
});
'''

You can also first instantiate a model and then save it.

'''js
...
```

#### <a name="apidoc.element.vogels.table.prototype.createTable"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>createTable (options, callback)](#apidoc.element.vogels.table.prototype.createTable)
- description and source-code
```javascript
createTable = function (options, callback) {
  var self = this;

  if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }
  var attributeDefinitions = [];

  attributeDefinitions.push(internals.attributeDefinition(self.schema, self.schema.hashKey));

  if(self.schema.rangeKey) {
    attributeDefinitions.push(internals.attributeDefinition(self.schema, self.schema.rangeKey));
  }

  var localSecondaryIndexes = [];

  _.forEach(self.schema.secondaryIndexes, function (params) {
    attributeDefinitions.push(internals.attributeDefinition(self.schema, params.rangeKey));
    localSecondaryIndexes.push(internals.secondaryIndex(self.schema, params));
  });

  var globalSecondaryIndexes = [];

  _.forEach(self.schema.globalIndexes, function (params, indexName) {

    if(!_.find(attributeDefinitions, { 'AttributeName': params.hashKey })) {
      attributeDefinitions.push(internals.attributeDefinition(self.schema, params.hashKey));
    }

    if(params.rangeKey && !_.find(attributeDefinitions, { 'AttributeName': params.rangeKey })) {
      attributeDefinitions.push(internals.attributeDefinition(self.schema, params.rangeKey));
    }

    globalSecondaryIndexes.push(internals.globalIndex(indexName, params));
  });

  var keySchema = internals.keySchema(self.schema.hashKey, self.schema.rangeKey);

  var params = {
    AttributeDefinitions : attributeDefinitions,
    TableName : self.tableName(),
    KeySchema : keySchema,
    ProvisionedThroughput : {
      ReadCapacityUnits : options.readCapacity || 1,
      WriteCapacityUnits : options.writeCapacity || 1
    }
  };

  if(localSecondaryIndexes.length >= 1) {
    params.LocalSecondaryIndexes = localSecondaryIndexes;
  }

  if(globalSecondaryIndexes.length >= 1) {
    params.GlobalSecondaryIndexes = globalSecondaryIndexes;
  }

  self.sendRequest('createTable', params, callback);
}
```
- example usage
```shell
...
  options = options || {};

  var tableName = model.tableName();

  model.describeTable(function (err, data) {
    if(_.isNull(data) || _.isUndefined(data)) {
      model.log.info('creating table: %s', tableName);
      return model.createTable(options, function (error) {

if(error) {
  model.log.warn({err : error}, 'failed to create table %s: %s', tableName, error);
  return callback(error);
}

model.log.info('waiting for table: %s to become ACTIVE', tableName);
...
```

#### <a name="apidoc.element.vogels.table.prototype.deleteTable"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>deleteTable (callback)](#apidoc.element.vogels.table.prototype.deleteTable)
- description and source-code
```javascript
deleteTable = function (callback) {
  callback = callback || _.noop;

  var params = {
    TableName : this.tableName(),
  };

  this.sendRequest('deleteTable', params, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.table.prototype.describeTable"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>describeTable (callback)](#apidoc.element.vogels.table.prototype.describeTable)
- description and source-code
```javascript
describeTable = function (callback) {

  var params = {
    TableName : this.tableName(),
  };

  this.sendRequest('describeTable', params, callback);
}
```
- example usage
```shell
...
var internals = {};

internals.createTable = function (model, options, callback) {
  options = options || {};

  var tableName = model.tableName();

  model.describeTable(function (err, data) {
    if(_.isNull(data) || _.isUndefined(data)) {
      model.log.info('creating table: %s', tableName);
      return model.createTable(options, function (error) {

if(error) {
  model.log.warn({err : error}, 'failed to create table %s: %s', tableName, error);
  return callback(error);
...
```

#### <a name="apidoc.element.vogels.table.prototype.destroy"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>destroy (hashKey, rangeKey, options, callback)](#apidoc.element.vogels.table.prototype.destroy)
- description and source-code
```javascript
destroy = function (hashKey, rangeKey, options, callback) {
  var self = this;

  if (_.isPlainObject(rangeKey) && typeof options === 'function' && !callback) {
    callback = options;
    options = rangeKey;
    rangeKey = null;
  } else if (typeof rangeKey === 'function' && !callback) {
    callback = rangeKey;
    options = {};
    rangeKey = null;
  } else if (_.isPlainObject(rangeKey) && !callback) {
    callback = options;
    options = rangeKey;
    rangeKey = null;
  } else if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  callback = callback || _.noop;
  options = options || {};

  if (_.isPlainObject(hashKey)) {
    rangeKey = hashKey[self.schema.rangeKey] || null;
    hashKey = hashKey[self.schema.hashKey];
  }

  var params = {
    TableName : self.tableName(),
    Key : self.serializer.buildKey(hashKey, rangeKey, self.schema)
  };

  if (options.expected) {
    internals.addConditionExpression(params, options.expected);

    delete options.expected;
  }

  params = _.merge({}, params, options);

  self.sendRequest('delete', params, function (err, data) {
    if(err) {
      return callback(err);
    }

    var item = null;
    if(data.Attributes) {
      item = self.initItem(self.serializer.deserializeItem(data.Attributes));
    }

    self._after.emit('destroy', item);
    return callback(null, item);
  });
}
```
- example usage
```shell
...
'''

### Deleting
You delete items in DynamoDB using the hashkey of model
If your model uses both a hash and range key, than both need to be provided

'''js
Account.destroy('foo@example.com', function (err) {
  console.log('account deleted');
});

// Destroy model using hash and range key
BlogPost.destroy('foo@example.com', 'Hello World!', function (err) {
  console.log('post deleted')
});
...
```

#### <a name="apidoc.element.vogels.table.prototype.get"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>get (hashKey, rangeKey, options, callback)](#apidoc.element.vogels.table.prototype.get)
- description and source-code
```javascript
get = function (hashKey, rangeKey, options, callback) {
  var self = this;

  if (_.isPlainObject(rangeKey) && typeof options === 'function' && !callback) {
    callback = options;
    options = rangeKey;
    rangeKey = null;
  } else if (typeof rangeKey === 'function' && !callback) {
    callback = rangeKey;
    options = {};
    rangeKey = null;
  } else if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  var params = {
    TableName : self.tableName(),
    Key : self.serializer.buildKey(hashKey, rangeKey, self.schema)
  };

  params = _.merge({}, params, options);

  self.sendRequest('get', params, function (err, data) {
    if(err) {
      return callback(err);
    }

    var item = null;
    if(data.Item) {
      item = self.initItem(self.serializer.deserializeItem(data.Item));
    }

    return callback(null, item);
  });
}
```
- example usage
```shell
...
'''

### Saving Models to DynamoDB
With your models defined, we can start saving them to DynamoDB.

'''js
Account.create({email: 'foo@example.com', name: 'Foo Bar', age: 21}, function (err, acc) {
  console.log('created account in DynamoDB', acc.get('email'));
});
'''

You can also first instantiate a model and then save it.

'''js
var acc = new Account({email: 'test@example.com', name: 'Test Example'});
...
```

#### <a name="apidoc.element.vogels.table.prototype.initItem"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>initItem (attrs)](#apidoc.element.vogels.table.prototype.initItem)
- description and source-code
```javascript
initItem = function (attrs) {
  var self = this;

  if(self.itemFactory) {
    return new self.itemFactory(attrs);
  } else {
    return new Item(attrs, self);
  }
}
```
- example usage
```shell
...
    if(err) {
      return callback(err);
    }

    var dynamoItems = data.Responses[table.tableName()];

    var items = _.map(dynamoItems, function(i) {
      return table.initItem(serializer.deserializeItem(i));
    });

    return callback(null, items);
  });
};

internals.getItems = function (table, serializer) {
...
```

#### <a name="apidoc.element.vogels.table.prototype.parallelScan"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>parallelScan (totalSegments)](#apidoc.element.vogels.table.prototype.parallelScan)
- description and source-code
```javascript
parallelScan = function (totalSegments) {
  var self = this;

  return new ParallelScan(self, self.serializer, totalSegments);
}
```
- example usage
```shell
...
The only difference is you must provide the total number of segments

**Caution** you can easily consume all your provisioned throughput with this api

'''js
var totalSegments = 8;

Account.parallelScan(totalSegments)
.where('age').gte(18)
.attributes('age')
.exec(callback);

// Load All accounts
Account
.parallelScan(totalSegments)
...
```

#### <a name="apidoc.element.vogels.table.prototype.query"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>query (hashKey)](#apidoc.element.vogels.table.prototype.query)
- description and source-code
```javascript
query = function (hashKey) {
  var self = this;

  return new Query(hashKey, self, self.serializer);
}
```
- example usage
```shell
...
### Query
For models that use hash and range keys Vogels provides a flexible and
chainable query api

'''js
// query for blog posts by werner@example.com
BlogPost
.query('werner@example.com')
.exec(callback);

// same as above, but load all results
BlogPost
.query('werner@example.com')
.loadAll()
.exec(callback);
...
```

#### <a name="apidoc.element.vogels.table.prototype.runBatchGetItems"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>runBatchGetItems (params, callback)](#apidoc.element.vogels.table.prototype.runBatchGetItems)
- description and source-code
```javascript
runBatchGetItems = function (params, callback) {

  var self = this;
  self.sendRequest('batchGet', params, callback);
}
```
- example usage
```shell
...
};

internals.paginatedRequest = function (request, table, callback) {
  var responses = [];

  var doFunc = function (callback) {

    table.runBatchGetItems(request, function (err, resp) {
if(err && err.retryable) {
  return callback();
} else if(err) {
  return callback(err);
}

request = resp.UnprocessedKeys;
...
```

#### <a name="apidoc.element.vogels.table.prototype.runQuery"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>runQuery (params, callback)](#apidoc.element.vogels.table.prototype.runQuery)
- description and source-code
```javascript
runQuery = function (params, callback) {
  var self = this;

  self.sendRequest('query', params, internals.deserializeItems(self, callback));
}
```
- example usage
```shell
...

Query.prototype.exec = function(callback) {
var self = this;

this.addKeyCondition(this.buildKey());

var runQuery = function (params, callback) {
  self.table.runQuery(params, callback);
};

return utils.paginatedRequest(self, runQuery, callback);
};

Query.prototype.buildKey = function () {
var key = this.table.schema.hashKey;
...
```

#### <a name="apidoc.element.vogels.table.prototype.runScan"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>runScan (params, callback)](#apidoc.element.vogels.table.prototype.runScan)
- description and source-code
```javascript
runScan = function (params, callback) {
  var self = this;

  self.sendRequest('scan', params, internals.deserializeItems(self, callback));
}
```
- example usage
```shell
...
return this;
};

Scan.prototype.exec = function(callback) {
var self = this;

var runScan = function (params, callback) {
  self.table.runScan(params, callback);
};

return utils.paginatedRequest(self, runScan, callback);
};

Scan.prototype.loadAll = function () {
this.options.loadAll = true;
...
```

#### <a name="apidoc.element.vogels.table.prototype.scan"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>scan ()](#apidoc.element.vogels.table.prototype.scan)
- description and source-code
```javascript
scan = function () {
  var self = this;

  return new Scan(self, self.serializer);
}
```
- example usage
```shell
...

### Scan
Vogels provides a flexible and chainable api for scanning over all your items
This api is very similar to the query api.

'''js
// scan all accounts, returning the first page or results
Account.scan().exec(callback);

// scan all accounts, this time loading all results
// note this will potentially make several calls to DynamoDB
// in order to load all results
Account
.scan()
.loadAll()
...
```

#### <a name="apidoc.element.vogels.table.prototype.sendRequest"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>sendRequest (method, params, callback)](#apidoc.element.vogels.table.prototype.sendRequest)
- description and source-code
```javascript
sendRequest = function (method, params, callback) {
  var self = this;

  var driver;
  if (_.isFunction(self.docClient[method])) {
    driver = self.docClient;
  } else if (_.isFunction(self.docClient.service[method])) {
    driver = self.docClient.service;
  }

  var startTime = Date.now();

  self.log.info({params : params}, 'vogels %s request', method.toUpperCase());
  driver[method].call(driver, params, function (err, data) {
    var elapsed = Date.now() - startTime;

    if (err) {
      self.log.warn({err : err}, 'vogels %s error', method.toUpperCase());
      return callback(err);
    } else {
      self.log.info({data : data}, 'vogels %s response - %sms', method.toUpperCase(), elapsed);
      return callback(null, data);
    }
  });
}
```
- example usage
```shell
...
  var params = {
TableName : self.tableName(),
Key : self.serializer.buildKey(hashKey, rangeKey, self.schema)
  };

  params = _.merge({}, params, options);

  self.sendRequest('get', params, function (err, data) {
if(err) {
  return callback(err);
}

var item = null;
if(data.Item) {
  item = self.initItem(self.serializer.deserializeItem(data.Item));
...
```

#### <a name="apidoc.element.vogels.table.prototype.tableName"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>tableName ()](#apidoc.element.vogels.table.prototype.tableName)
- description and source-code
```javascript
tableName = function () {
  if(this.schema.tableName) {
    if(_.isFunction(this.schema.tableName)) {
      return this.schema.tableName.call(this);
    } else {
      return this.schema.tableName;
    }
  } else {
    return this.config.name;
  }
}
```
- example usage
```shell
...
};

var resulsFunc = function (err) {
  if(err) {
    return callback(err);
  }

  callback(null, internals.mergeResponses(table.tableName(), responses));
};

async.doWhilst(doFunc, testFunc, resulsFunc);
};

internals.buckets = function (keys) {
var buckets = [];
...
```

#### <a name="apidoc.element.vogels.table.prototype.update"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>update (item, options, callback)](#apidoc.element.vogels.table.prototype.update)
- description and source-code
```javascript
update = function (item, options, callback) {
  var self = this;

  if (typeof options === 'function' && !callback) {
    callback = options;
    options = {};
  }

  callback = callback || _.noop;
  options = options || {};

  var start = function (callback) {
    var paramName = _.isString(self.schema.updatedAt) ? self.schema.updatedAt : 'updatedAt';

    if(self.schema.timestamps && self.schema.updatedAt !== false && !_.has(item, paramName)) {
      item[paramName] = new Date().toISOString();
    }

    return callback(null, item);
  };

  internals.callBeforeHooks(self, 'update', start, function (err, data) {
    if(err) {
      return callback(err);
    }

    var hashKey = data[self.schema.hashKey];
    var rangeKey = data[self.schema.rangeKey] || null;

    var params = {
      TableName : self.tableName(),
      Key : self.serializer.buildKey(hashKey, rangeKey, self.schema),
      ReturnValues : 'ALL_NEW'
    };

    var exp = internals.updateExpressions(self.schema, data, options);

    if(exp.UpdateExpression) {
      params.UpdateExpression = exp.UpdateExpression;
      delete options.UpdateExpression;
    }

    if(exp.ExpressionAttributeValues) {
      params.ExpressionAttributeValues = exp.ExpressionAttributeValues;
      delete options.ExpressionAttributeValues;
    }

    if(exp.ExpressionAttributeNames) {
      params.ExpressionAttributeNames = exp.ExpressionAttributeNames;
      delete options.ExpressionAttributeNames;
    }

    if (options.expected) {
      internals.addConditionExpression(params, options.expected);
      delete options.expected;
    }

    params = _.chain({}).merge(params, options).omit(_.isEmpty).value();

    self.sendRequest('update', params, function (err, data) {
      if(err) {
        return callback(err);
      }

      var result = null;
      if(data.Attributes) {
        result = self.initItem(self.serializer.deserializeItem(data.Attributes));
      }

      self._after.emit('update', result);
      return callback(null, result);
    });

  });
}
```
- example usage
```shell
...
vogels.AWS.config.loadFromPath('credentials.json');
'''

When running on EC2 its recommended to leverage EC2 IAM roles. If you have configured your instance to use IAM roles, Vogels will
 automatically select these credentials for use in your application, and you do not need to manually provide credentials in any
other format.

'''js
var vogels = require('vogels');
vogels.AWS.config.update({region: "REGION"}); // region must be set
'''

You can also directly pass in your access key id, secret and region.
  * Its recommend you not hard-code credentials inside an application. Use this method only for small personal scripts or for testing
 purposes.

'''js
var vogels = require('vogels');
...
```

#### <a name="apidoc.element.vogels.table.prototype.updateTable"></a>[function <span class="apidocSignatureSpan">vogels.table.prototype.</span>updateTable (throughput, callback)](#apidoc.element.vogels.table.prototype.updateTable)
- description and source-code
```javascript
updateTable = function (throughput, callback) {
  var self = this;
  if (typeof throughput === 'function' && !callback) {
    callback = throughput;
    throughput = {};
  }

  callback = callback || _.noop;
  throughput = throughput || {};

  async.parallel([
    async.apply(internals.syncIndexes, self),
    async.apply(internals.updateTableCapacity, self, throughput),
  ], callback);
}
```
- example usage
```shell
...
  return callback(error);
}

model.log.info('waiting for table: %s to become ACTIVE', tableName);
internals.waitTillActive(model, callback);
      });
    } else {
      model.updateTable(function (err) {
if(err) {
  model.log.warn({err : err}, 'failed to update table %s: %s', tableName, err);
  return callback(err);
}

model.log.info('waiting for table: %s to become ACTIVE', tableName);
internals.waitTillActive(model, callback);
...
```



# <a name="apidoc.module.vogels.types"></a>[module vogels.types](#apidoc.module.vogels.types)

#### <a name="apidoc.element.vogels.types.binarySet"></a>[function <span class="apidocSignatureSpan">vogels.types.</span>binarySet ()](#apidoc.element.vogels.types.binarySet)
- description and source-code
```javascript
binarySet = function () {
  var set = Joi.array().includes(Joi.binary(), Joi.string()).meta({dynamoType : 'BS'});
  return set;
}
```
- example usage
```shell
...
case 'B':
  return serialize.binary(value);
case 'NS':
  return serialize.numberSet(value);
case 'SS':
  return serialize.stringSet(value);
case 'BS':
  return serialize.binarySet(value);
default:
  return value;
}
};

serializer.buildKey = function (hashKey, rangeKey, schema) {
var obj = {};
...
```

#### <a name="apidoc.element.vogels.types.numberSet"></a>[function <span class="apidocSignatureSpan">vogels.types.</span>numberSet ()](#apidoc.element.vogels.types.numberSet)
- description and source-code
```javascript
numberSet = function () {
  var set = Joi.array().includes(Joi.number()).meta({dynamoType : 'NS'});
  return set;
}
```
- example usage
```shell
...
case 'DATE':
  return serialize.date(value);
case 'BOOL':
  return serialize.boolean(value);
case 'B':
  return serialize.binary(value);
case 'NS':
  return serialize.numberSet(value);
case 'SS':
  return serialize.stringSet(value);
case 'BS':
  return serialize.binarySet(value);
default:
  return value;
}
...
```

#### <a name="apidoc.element.vogels.types.stringSet"></a>[function <span class="apidocSignatureSpan">vogels.types.</span>stringSet ()](#apidoc.element.vogels.types.stringSet)
- description and source-code
```javascript
stringSet = function () {
  var set = Joi.array().includes(Joi.string()).meta({dynamoType : 'SS'});

  return set;
}
```
- example usage
```shell
...
  // add the timestamp attributes (updatedAt, createdAt)
  timestamps : true,

  schema : {
    email   : Joi.string().email(),
    name    : Joi.string(),
    age     : Joi.number(),
    roles   : vogels.types.stringSet(),
    settings : {
      nickname      : Joi.string(),
      acceptedTerms : Joi.boolean().default(false)
    }
  }
});
'''
...
```

#### <a name="apidoc.element.vogels.types.timeUUID"></a>[function <span class="apidocSignatureSpan">vogels.types.</span>timeUUID ()](#apidoc.element.vogels.types.timeUUID)
- description and source-code
```javascript
timeUUID = function () {
  return Joi.string().guid().default(nodeUUID.v1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vogels.types.uuid"></a>[function <span class="apidocSignatureSpan">vogels.types.</span>uuid ()](#apidoc.element.vogels.types.uuid)
- description and source-code
```javascript
uuid = function () {
  return Joi.string().guid().default(nodeUUID.v4);
}
```
- example usage
```shell
...
the model in DynamoDB.

'''js
var Tweet = vogels.define('Tweet', {
  hashKey : 'TweetID',
  timestamps : true,
  schema : {
    TweetID : vogels.types.uuid(),
    content : Joi.string(),
  }
});
'''

### Configuration
You can configure vogels to automatically add 'createdAt' and 'updatedAt' timestamp attributes when
...
```



# <a name="apidoc.module.vogels.utils"></a>[module vogels.utils](#apidoc.module.vogels.utils)

#### <a name="apidoc.element.vogels.utils.mergeResults"></a>[function <span class="apidocSignatureSpan">vogels.utils.</span>mergeResults (responses, tableName)](#apidoc.element.vogels.utils.mergeResults)
- description and source-code
```javascript
mergeResults = function (responses, tableName) {
  var result = {
    Items : [],
    ConsumedCapacity : {
      CapacityUnits : 0,
      TableName : tableName
    },
    Count : 0,
    ScannedCount : 0
  };

  var merged = _.reduce(responses, function (memo, resp) {
    if(!resp) {
      return memo;
    }

    memo.Count += resp.Count || 0;
    memo.ScannedCount += resp.ScannedCount || 0;

    if(resp.ConsumedCapacity) {
      memo.ConsumedCapacity.CapacityUnits += resp.ConsumedCapacity.CapacityUnits || 0;
    }

    if(resp.Items) {
      memo.Items = memo.Items.concat(resp.Items);
    }

    if(resp.LastEvaluatedKey) {
      memo.LastEvaluatedKey = resp.LastEvaluatedKey;
    }

    return memo;
  }, result);

  if(merged.ConsumedCapacity.CapacityUnits === 0) {
    delete merged.ConsumedCapacity;
  }

  if(merged.ScannedCount === 0) {
    delete merged.ScannedCount;
  }

  return merged;
}
```
- example usage
```shell
...

  async.parallel(scanFuncs, function (err, responses) {
    if(err) {
      return callback(err);
    }

    combinedStream.push(null);
    return callback(null, utils.mergeResults(responses, self.table.tableName()));
  });
};

if(streamMode) {
  combinedStream._read = startScans;
} else {
  startScans();
...
```

#### <a name="apidoc.element.vogels.utils.omitNulls"></a>[function <span class="apidocSignatureSpan">vogels.utils.</span>omitNulls (data)](#apidoc.element.vogels.utils.omitNulls)
- description and source-code
```javascript
omitNulls = function (data) {
  return _.omit(data, function(value) {
    return _.isNull(value) ||
      _.isUndefined(value) ||
      (_.isArray(value) && _.isEmpty(value)) ||
      (_.isString(value) && _.isEmpty(value));
  });
}
```
- example usage
```shell
...

var result = self.schema.validate(data);

if(result.error) {
  return callback(result.error);
}

var attrs = utils.omitNulls(data);

var params = {
  TableName : self.tableName(),
  Item : self.serializer.serializeItem(self.schema, attrs)
};

if (options.expected) {
...
```

#### <a name="apidoc.element.vogels.utils.omitPrimaryKeys"></a>[function <span class="apidocSignatureSpan">vogels.utils.</span>omitPrimaryKeys (schema, params)](#apidoc.element.vogels.utils.omitPrimaryKeys)
- description and source-code
```javascript
omitPrimaryKeys = function (schema, params) {
  return _.omit(params, schema.hashKey, schema.rangeKey);
}
```
- example usage
```shell
...
  return result;
}, {});
};

exports.serializeUpdateExpression = function (schema, item) {
var datatypes = schema._modelDatatypes;

var data = utils.omitPrimaryKeys(schema, item);

var memo = {
  expressions : {},
  attributeNames : {},
  values : {},
};
...
```

#### <a name="apidoc.element.vogels.utils.paginatedRequest"></a>[function <span class="apidocSignatureSpan">vogels.utils.</span>paginatedRequest (self, runRequestFunc, callback)](#apidoc.element.vogels.utils.paginatedRequest)
- description and source-code
```javascript
paginatedRequest = function (self, runRequestFunc, callback) {
  // if callback isn't passed switch to stream
  if(!callback) {
    return utils.streamRequest(self, runRequestFunc);
  }

  var lastEvaluatedKey = null;
  var responses = [];
  var retry = false;

  var doFunc = function (callback) {
    if(lastEvaluatedKey) {
      self.startKey(lastEvaluatedKey);
    }

    runRequestFunc(self.buildRequest(), function (err, resp) {
      if(err && err.retryable) {
        retry = true;
        return setImmediate(callback);
      } else if(err) {
        retry = false;
        return setImmediate(callback, err);
      }

      retry = false;
      lastEvaluatedKey = resp.LastEvaluatedKey;

      responses.push(resp);

      return setImmediate(callback);
    });
  };

  var testFunc = function () {
    return (self.options.loadAll && lastEvaluatedKey) || retry;
  };

  var resulsFunc = function (err) {
    if(err) {
      return callback(err);
    }

    return callback(null, utils.mergeResults(responses, self.table.tableName()));
  };

  async.doWhilst(doFunc, testFunc, resulsFunc);
}
```
- example usage
```shell
...
};

internals.initialBatchGetItems = function (keys, table, serializer, options, callback) {
  var serializedKeys = internals.serializeKeys(keys, table, serializer);

  var request = internals.buildInitialGetItemsRequest(table.tableName(), serializedKeys, options);

  internals.paginatedRequest(request, table, function (err, data) {
if(err) {
  return callback(err);
}

var dynamoItems = data.Responses[table.tableName()];

var items = _.map(dynamoItems, function(i) {
...
```

#### <a name="apidoc.element.vogels.utils.strToBin"></a>[function <span class="apidocSignatureSpan">vogels.utils.</span>strToBin (value)](#apidoc.element.vogels.utils.strToBin)
- description and source-code
```javascript
strToBin = function (value) {
  if (typeof(value) !== 'string') {
    var StrConversionError = 'Need to pass in string primitive to be converted to binary.';
    throw new Error(StrConversionError);
  }

  if (AWS.util.isBrowser()) {
    var len = value.length;
    var bin = new Uint8Array(new ArrayBuffer(len));
    for (var i = 0; i < len; i++) {
      bin[i] = value.charCodeAt(i);
    }
    return bin;
  } else {
    return AWS.util.Buffer(value);
  }
}
```
- example usage
```shell
...
}
};

var serialize = internals.serialize = {

binary: function (value) {
  if(_.isString(value)) {
    return utils.strToBin(value);
  }

  return value;
},

date : function (value) {
  if(_.isDate(value)) {
...
```

#### <a name="apidoc.element.vogels.utils.streamRequest"></a>[function <span class="apidocSignatureSpan">vogels.utils.</span>streamRequest (self, runRequestFunc)](#apidoc.element.vogels.utils.streamRequest)
- description and source-code
```javascript
streamRequest = function (self, runRequestFunc) {
  var lastEvaluatedKey = null;
  var performRequest = true;

  var stream = new Readable({objectMode: true});

  var startRead = function () {
    if(!performRequest) {
      return;
    }

    if(lastEvaluatedKey) {
      self.startKey(lastEvaluatedKey);
    }

    runRequestFunc(self.buildRequest(), function (err, resp) {
      if(err && err.retryable) {
        return setTimeout(startRead, 1000);
      } else if(err) {
        return stream.emit('error', err);
      } else {
        lastEvaluatedKey = resp.LastEvaluatedKey;

        if(!self.options.loadAll || !lastEvaluatedKey) {
          performRequest = false;
        }

        stream.push(resp);

        if(!self.options.loadAll || !lastEvaluatedKey) {
          stream.push(null);
        }
      }

    });
  };

  stream._read = function () {
    startRead();
  };

  return stream;
}
```
- example usage
```shell
...

return merged;
};

utils.paginatedRequest = function (self, runRequestFunc, callback) {
// if callback isn't passed switch to stream
if(!callback) {
  return utils.streamRequest(self, runRequestFunc);
}

var lastEvaluatedKey = null;
var responses = [];
var retry = false;

var doFunc = function (callback) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
