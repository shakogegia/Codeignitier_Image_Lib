Codeignitier_Image_resize_and_crop
==================================

Codeignitier Image resize and crop library

Instalation
==================================
Just put Resize_class.php file in your library folder

Usage
==================================
<pre>
<code>
  $imageLink = '/images/sample.jpg';
  $imageTarget = '/images/sample_resized.jpg';
  
  // *** 0) Load Resize Library
  $this->load->library('resize_class');
  // *** 1) Start 
  $this->resize_class->start($imageLink);
  // *** 2) Resize image (1-width, 2-height, 3-options: exact, portrait, landscape, auto, crop)
  $this->resize_class->resizeImage(216, 223, 'crop');
  // *** 3) Save image (1-directory, 2-quality)
  $this->resize_class->saveImage($imageTarget, 100);
</code>
</pre>
