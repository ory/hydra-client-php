# # Certificate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authorityKeyId** | **int[]** | authority key Id | [optional] 
**basicConstraintsValid** | **bool** | BasicConstraintsValid indicates whether IsCA, MaxPathLen, and MaxPathLenZero are valid. | [optional] 
**cRLDistributionPoints** | **string[]** | CRL Distribution Points | [optional] 
**dNSNames** | **string[]** | Subject Alternate Name values. (Note that these values may not be valid if invalid values were contained within a parsed certificate. For example, an element of DNSNames may not be a valid DNS domain name.) | [optional] 
**emailAddresses** | **string[]** | email addresses | [optional] 
**excludedDNSDomains** | **string[]** | excluded DNS domains | [optional] 
**excludedEmailAddresses** | **string[]** | excluded email addresses | [optional] 
**excludedIPRanges** | [**\Ory\Hydra\Client\Model\IPNet[]**](IPNet.md) | excluded IP ranges | [optional] 
**excludedURIDomains** | **string[]** | excluded URI domains | [optional] 
**extKeyUsage** | **int[]** | ext key usage | [optional] 
**extensions** | [**\Ory\Hydra\Client\Model\Extension[]**](Extension.md) | Extensions contains raw X.509 extensions. When parsing certificates, this can be used to extract non-critical extensions that are not parsed by this package. When marshaling certificates, the Extensions field is ignored, see ExtraExtensions. | [optional] 
**extraExtensions** | [**\Ory\Hydra\Client\Model\Extension[]**](Extension.md) | ExtraExtensions contains extensions to be copied, raw, into any marshaled certificates. Values override any extensions that would otherwise be produced based on the other fields. The ExtraExtensions field is not populated when parsing certificates, see Extensions. | [optional] 
**iPAddresses** | [**\Ory\Hydra\Client\Model\array[]**](array.md) | IP addresses | [optional] 
**isCA** | **bool** | is c a | [optional] 
**issuer** | [**\Ory\Hydra\Client\Model\Name**](Name.md) |  | [optional] 
**issuingCertificateURL** | **string[]** | issuing certificate URL | [optional] 
**keyUsage** | **int** | KeyUsage KeyUsage KeyUsage KeyUsage represents the set of actions that are valid for a given key. It&#39;s a bitmap of the KeyUsage* constants. | [optional] 
**maxPathLen** | **int** | MaxPathLen and MaxPathLenZero indicate the presence and value of the BasicConstraints&#39; \&quot;pathLenConstraint\&quot;.  When parsing a certificate, a positive non-zero MaxPathLen means that the field was specified, -1 means it was unset, and MaxPathLenZero being true mean that the field was explicitly set to zero. The case of MaxPathLen&#x3D;&#x3D;0 with MaxPathLenZero&#x3D;&#x3D;false should be treated equivalent to -1 (unset).  When generating a certificate, an unset pathLenConstraint can be requested with either MaxPathLen &#x3D;&#x3D; -1 or using the zero value for both MaxPathLen and MaxPathLenZero. | [optional] 
**maxPathLenZero** | **bool** | MaxPathLenZero indicates that BasicConstraintsValid&#x3D;&#x3D;true and MaxPathLen&#x3D;&#x3D;0 should be interpreted as an actual maximum path length of zero. Otherwise, that combination is interpreted as MaxPathLen not being set. | [optional] 
**notBefore** | [**\DateTime**](\DateTime.md) | not before Format: date-time Format: date-time Format: date-time | [optional] 
**oCSPServer** | **string[]** | RFC 5280, 4.2.2.1 (Authority Information Access) | [optional] 
**permittedDNSDomains** | **string[]** | permitted DNS domains | [optional] 
**permittedDNSDomainsCritical** | **bool** | Name constraints | [optional] 
**permittedEmailAddresses** | **string[]** | permitted email addresses | [optional] 
**permittedIPRanges** | [**\Ory\Hydra\Client\Model\IPNet[]**](IPNet.md) | permitted IP ranges | [optional] 
**permittedURIDomains** | **string[]** | permitted URI domains | [optional] 
**policyIdentifiers** | [**\Ory\Hydra\Client\Model\array[]**](array.md) | policy identifiers | [optional] 
**publicKey** | [**object**](.md) | public key | [optional] 
**publicKeyAlgorithm** | **int** | PublicKeyAlgorithm PublicKeyAlgorithm PublicKeyAlgorithm public key algorithm | [optional] 
**raw** | **int[]** | raw | [optional] 
**rawIssuer** | **int[]** | raw issuer | [optional] 
**rawSubject** | **int[]** | raw subject | [optional] 
**rawSubjectPublicKeyInfo** | **int[]** | raw subject public key info | [optional] 
**rawTBSCertificate** | **int[]** | raw t b s certificate | [optional] 
**serialNumber** | [**object**](.md) | Operations always take pointer arguments (*Int) rather than Int values, and each unique Int value requires its own unique *Int pointer. To \&quot;copy\&quot; an Int value, an existing (or newly allocated) Int must be set to a new value using the Int.Set method; shallow copies of Ints are not supported and may lead to errors. | [optional] 
**signature** | **int[]** | signature | [optional] 
**signatureAlgorithm** | **int** | SignatureAlgorithm SignatureAlgorithm SignatureAlgorithm signature algorithm | [optional] 
**subject** | [**\Ory\Hydra\Client\Model\Name**](Name.md) |  | [optional] 
**subjectKeyId** | **int[]** | subject key Id | [optional] 
**uRIs** | [**\Ory\Hydra\Client\Model\URL[]**](URL.md) | u r is | [optional] 
**unhandledCriticalExtensions** | [**\Ory\Hydra\Client\Model\array[]**](array.md) | UnhandledCriticalExtensions contains a list of extension IDs that were not (fully) processed when parsing. Verify will fail if this slice is non-empty, unless verification is delegated to an OS library which understands all the critical extensions.  Users can access these extensions using Extensions and can remove elements from this slice if they believe that they have been handled. | [optional] 
**unknownExtKeyUsage** | [**\Ory\Hydra\Client\Model\array[]**](array.md) | unknown ext key usage | [optional] 
**version** | **int** | version | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)


