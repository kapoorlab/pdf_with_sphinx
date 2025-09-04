:author: Varun Kapoor
:email: varun.kapoor@kaporlabs.org
:institution: KapoorLabs, Paris, France.



:bibliography: vkc


------------------------------------------------------------------------------------------------
Title of the document
------------------------------------------------------------------------------------------------

.. class:: abstract


.. class:: keywords



Writing Equations
-----------------

This is how we can type labelled equations 

.. math::
   :label: eq-schrodinger-stationary

   \hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r})


For writing simple math stuff without numbering we can use 

:math:`GT = \{gt\}`, :math:`SEG=\{seg\}` are two sets of segmented objects.



Writing Code
-------------




.. code-block::   python

  def iou3D(box_unet, centroid_star):
    
    ndim = len(centroid_star)
    inside = False
    
    Condition = [Conditioncheck(centroid_star, box_unet,
     p, ndim)
     for p in range(0,ndim)]
        
    inside = all(Condition)
    
    return inside
  
  def Conditioncheck(centroid_centroid, box_unet, 
         p, ndim):

    condition = False

    if centroid_star[p] >= box_unet[p]
    and centroid_star[p] <= box_unet[p + ndim]:

         condition = True

    return condition

Putting a figure
------------------


For adding a figure it is like 

.. figure:: Figures/radiation.jpg
   :name: radiation

   Schematic representation showing the radiation spectrum with decreasing wavelength (in meters) from left to right, radio waves have wavelength of kilometers (that is what it needs to be in our houses from a transmitter tower), microwaves of about 5 cm (easy guess as the size of the box itself is about 15 cm or so) while the visible radiation is 400-800 nano meter.


Then we can refer to the figure by saying is shown in the Figure :ref:`radiation`



Citing People
--------------

:cite:`schmidt2018` :cite:`weigert2020` :cite:`Beucher2018` :cite:`Ronn2015` :cite:`Wolny2020` :cite:`eschweiler2018`

References
---------------------
