### Example Data Leak 

# Incident Summary 

A sales manager shared access to a folder of internal-only documents with their
team during a meeting. The folder contained files associated with a new product that has not been
publicly announced. It also included customer analytics and promotional materials. After the meeting,
the manager did not revoke access to the internal folder, but warned the team to wait for approval
before sharing the promotional materials with others.

During a video call with a business partner, a member of the sales team forgot the warning from their
manager. The sales representative intended to share a link to the promotional materials so that the
business partner could circulate the materials to their customers. However, the sales representative
accidentally shared a link to the internal folder instead. Later, the business partner posted the link on
their company's social media page assuming that it was the promotional materials.


| Control                              | Least privilege |
|--------------------------------------|-----------------|
| Issues                               | Access to the internal folder was not limited to the sales team and the
manager. The business partner should not have been given permission to
share the promotional information to social media.              |
| Review                               | NIST SP 800-53: AC-6 addresses how an organization can protect their data

privacy by implementing least privilege. It also suggests control
enhancements to improve the effectiveness of least privilege.  | 
| Recommendations                      |  The recommendation for this situation would be to ensure that only the minimal access and authorization requried to complete a task should be provided to employees. Changes should include Automatticlly revoking access to informaiton after a period of time and restricting access t osensitive resources based on user roles               |
| Justifications                       | Data leaks can be prevented if shared links to internal files are restricted to
employees only. Also, requiring managers and security teams to regularly
audit access to team files would help limit the exposure of sensitive
information.              |
