# Raven Authentication

This module contains a number of enhancements to aid configurability and make it easier to use Raven in complex senarios.  These configuration settings are available at admin/config/people/raven

## Settings

There is a Time Offset field, which can be used to provide an ajustment if authentication is failing on account of an inaccurate clock.  You can also deal with clock drift by checking the box to Use the universities ucs time servers to update the offset automatically.

The tolerance to incorrect/late time is configurable.  You should increase this if the server will be under heavy load, and reduce it if you want tighter security (at the expense of occasionally rejecting valid authentication claims.

If you are having lots of problems with all this, you can check the box to ignore timing completely, but this opens you up to man in the middle attacks so it is not recomended in any security critical aplication.

If you un-tick allow new users, only users you have specifically created will be accepted.  Regardlesss of whether this is ticked, you will be able to add users manually as long as their username matches their crsid it doesn't matter what their password is (You should probably make it something long and random and keep no record of it).  This is useful to configure permissions in advance.

## Disclaimer

This module is provided as is, neither the RCSA, nor the authors of this module accept any liability for errors it may cause.