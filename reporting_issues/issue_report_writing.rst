.. _doc_issue_report_writing:

How to write a good issue report
================================

If you already know what needs to go into an issue report and are interested in writing
issue reports that also get the attention of triagers and maintainers, you can skip ahead to
the :ref:`guide below <doc_grabbing_triager_attention>`.

The anatomy of an issue report
------------------------------

The basics
~~~~~~~~~~

If in doubt, list things like system details in case it might be relevant.

.. TODO: A basic description of each part of a report

The critical parts
~~~~~~~~~~~~~~~~~~

.. TODO: A summary

The issue description
^^^^^^^^^^^^^^^^^^^^^

The most important part of an issue report is the description of the issue. While clear steps
to reproduce the issue, or even an MRP, are great *additions* to a report they are not replacements
for a clear and detailed description of the issue.

When writing the description of your issue it's important that you cover the following:
- What is happening, try to get as much detail as possible to avoid confusion, and please keep in mind
  that what might be obvious to you might not be to everyone else. This should be described in text form
  if possible (see :ref:`below <doc_video_and_screenshots_in_reports>`__ for a note about video and screenshots).
- How you expect, or want, it to behave and work, it is important that we understand what you expect to happen
  and how you expect the engine to work, some times issues are caused by incorrect assumptions and expectations.
  These cases are still important, and some can result in changes to the way the engine behaves,
  or they might indicate that the documentation needs to be improved, or that the design of the editor might
  need to be adjusted to make it clear how things work, and how to make things happen.
- How the way it behaves conflicts with that expectation, even with a clear description of what happens,
  and how you expect it to behave, it might not always be clear exactly in what way the two don't align.

Having a clear description of the issue, and not relying on people replicating the issue to see what is going on,
helps in many ways. Many contributors can find the time to look through an issue and try to understand what is
going on even when they aren't able to dedicate the time to run an MRP or try to reproduce a bug. Many bugs are
solved without even running the editor by contributors figuring out what is happening from just the description.
A clear description also makes it easier to work out what is happening even when you can't test the bug yourself,
for example if it is a bug happening on a platform you don't have access to. And even when a bug requires actively
reproducing it yourself to solve it a clear description helps to get you on the right path, and more importantly
helps you confirm that what you are seeing when testing the issue is the same as what the author of the report is facing.

The reproduction steps
^^^^^^^^^^^^^^^^^^^^^^

.. TODO

The Minimum Reproduction Project (MRP)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A common misconception about the MRP is that its main goal is to "prove" that a bug is happening. But it is actually
far more useful in other ways, and someone making a bug report is proof enough that something is happening.

The main purpose of an MRP is to be able to reliably reproduce a bug, to be able to narrow down exactly how to make
the bug happen. This is important both because knowing how to make a bug happen easily is critical to finding what is
causing the issue, for example by being able to slightly adjust the MRP and see if it stops happening, or running on
a different platform to see if it still happens. And once you have figured out what is causing the bug, the MRP once again
comes in handy to help you make sure the bug *stops* happening after you've created a fix. The hardest kind of bug to fix is
a bug that you can't be sure if it stops happening because you fixed it, or because you just can't make it happen reliably.

.. TODO

.. _doc_video_and_screenshots_in_reports:

Video and screenshots in reports
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Adding screenshots or video of what is happening is a great way to add more detail to this, but behavior should,
if possible, be described in text as well to make sure everyone understands and that everyone can access the information.
It can also be hard to judge if something is obvious from a video when you already know what it looks like.
Not only is this important for accessibility reasons, but some video formats are unavailable on some platforms,
especially in mobile browsers. The links to video files or screenshots can also become dead over time meaning
the information gets lost, this cannot happen to text descriptions. It is also not possible to search for information
in images or videos making it much harder to discover existing issues when reporting.

Code should *always* be posted as text (using the code formatting tags [add details]), unless the issue is not about the
code itself, for example if it is about syntax highlighting etc. Error messages should also always be provided in text form
rather than image or video, this is for multiple reasons, including the ones listed in the previous paragraph.

Having clear details of an error message can be enough to solve an issue. Especially if the error message is very specific.
It is, after all, the very reason error messages even exist, to give clear information that users and maintainers can use
to work out what is wrong.

.. _doc_grabbing_triager_attention:

How to grab triager attention
-----------------------------

.. TODO
